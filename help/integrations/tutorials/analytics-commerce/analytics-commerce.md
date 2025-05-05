---
title: Integrar [!DNL Analytics] con [!DNL Commerce] tutorial
description: Aprenda a integrar [!DNL Analytics] con [!DNL Commerce].
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Integrar [!DNL Analytics] con [!DNL Commerce]

## Incorporación inicial

Estas instrucciones están destinadas a los proyectos hospedados en la nube de Adobe [!DNL Commerce]. El alojamiento propio puede variar hasta cierto punto, pero el proceso general debe ser similar.

1. Compruebe el código en su entorno local
1. Usar el módulo Compositor e instalación
1. Siga las instrucciones individuales aquí y vuelva cuando haya terminado para finalizar los pasos restantes
   [Instalar y configurar el conector Experience [!DNL Platform] connector](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Confirme el archivo composer.json y, si se encuentra en la nube, los archivos composer.lock.
1. Compruebe que el módulo esté en los entornos de ensayo o producción
Para ello, inicie sesión en la sección de administración del Adobe [!DNL Commerce] y busque estas secciones nuevas en Sistema > Servicios
   ![Extensión del conector [!DNL Platform] de la experiencia](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Configure el módulo con sus credenciales desde el back office de la Adobe [!DNL Commerce].
   * Primero configure el conector de servicios [!DNL Commerce], como se muestra a continuación.

     Configuración de ![[!DNL Commerce] Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * A continuación, seleccione la configuración del conector Experience [!DNL Platform], como se muestra a continuación.

     ![Conector de experiencia [!DNL Platform]](./assets/analytics-commerce/experience-platform-connector.png)

Para obtener más información sobre cada fase y paso del proceso de incorporación, sigue las instrucciones de la [descripción general del conector Experience [!DNL Platform] 2&rbrace;. ](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"} El tutorial del conector Experience [!DNL Platform] cubre cada sección en profundidad y responde a las preguntas que pueda tener. Utilice este tutorial para el resto de los pasos de configuración rápida.

## Configuración de Experience Edge y el Adobe [!DNL Analytics]

1. Compruebe que su organización tiene acceso al Adobe [!DNL Analytics] (y usted lo tiene). Para confirmarlo, vaya a la [página principal de Adobe Experience Cloud](https://experience.adobe.com/) y haga clic en el conmutador de aplicaciones (nueve puntos) en la barra de navegación superior.

1. Cree un nuevo grupo de informes en el Adobe [!DNL Analytics] o identifique el identificador del grupo de informes en el que va a insertar los datos de [!DNL Commerce]. Para obtener más información, vea un tutorial sobre [crear un nuevo grupo de informes](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). Necesitará este ID de grupo de informes en el paso del conjunto de datos a continuación.

1. Vaya a la [experiencia de Adobe [!DNL Platform] interfaz](https://platform.adobe.com) si tiene acceso a la experiencia [!DNL Platform]. Si no tiene acceso a esa interfaz, puede realizar todos los pasos necesarios que se enumeran a continuación en la Experiencia de Adobe [!DNL Platform] [Interfaz de recopilación de datos](https://experience.adobe.com/#/data-collection).

1. Cree o actualice su esquema XDM con [!DNL Commerce] grupos de campos específicos. Para obtener más información sobre cómo crear un esquema, consulte el tutorial [&quot;Crear esquemas&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=es).
   * Deberá seleccionar este esquema de las opciones del paso del conjunto de datos a continuación. Para crear un esquema, mire en la columna izquierda debajo de **Administración de datos** y busque **Esquemas**. Ahora, en la parte superior derecha de la interfaz, haga clic en **Crear esquema**. Seleccione ExperienceEvent de XDM.
   * Después de crear un nuevo esquema, agregará los [!DNL Commerce] grupos de campos. En el lado izquierdo de la interfaz de usuario, busque Grupos de campos y haga clic en **Agregar**
      * En la búsqueda, puede filtrar escribiendo `ExperienceEvent Commerce`
      * Seleccione el **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** marcando la casilla
      * A continuación, haga clic en **Agregar grupos de campos** en la parte superior derecha para guardar y continuar

1. De forma opcional (y solo si está en la interfaz de Experience [!DNL Platform]): cree un nuevo conjunto de datos
   * Este paso le permite llevar los datos de [!DNL Commerce] a la experiencia [!DNL Platform] (por separado de llevar los datos al Adobe [!DNL Analytics]). Realice este paso si tiene acceso a la experiencia [!DNL Platform] y planea utilizar los datos de [!DNL Commerce] en las aplicaciones compatibles con Experience [!DNL Platform], como Real-Time Customer Data [!DNL Platform], Customer Recorrido [!DNL Analytics] o Journey Optimizer.
   * Deberá seleccionar este conjunto de datos de las opciones del paso de secuencia de datos a continuación.
   * En el encabezado de la columna izquierda **Administración de datos** en la navegación izquierda, seleccione **Conjuntos de datos**.
   * Haga clic en **Crear conjunto de datos** en la parte superior derecha. Elija la opción **Crear conjunto de datos a partir del esquema**.
   * Busque y utilice el esquema que ha creado en el último paso

1. Crear la secuencia de datos para enviar los datos de [!DNL Commerce] al Adobe [!DNL Analytics]
   * Bajo el encabezado **Recopilación de datos** en la columna izquierda, seleccione **Flujos de datos**.
   * Haga clic en **Nueva secuencia de datos** en la parte superior derecha de la interfaz.
   * Proporcione un nombre y una descripción opcional.
   * Busque y seleccione el esquema que ha creado o identificado en el paso anterior.
   * Añada las opciones avanzadas que desee. Para obtener más información acerca de las opciones avanzadas, visite la [documentación](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=es).
   * Haga clic en **Guardar** para continuar.
   * Haga clic en **Agregar servicio** y elija **Adobe[!DNL Analytics]** en el campo desplegable.
   * Haga clic en **Agregar grupo de informes** e introduzca el ID del grupo de informes que creó o identificó en un paso anterior. Puede agregar más de un grupo de informes si desea que los datos fluyan a varios grupos de informes.
   * Opcionalmente, y si creó un conjunto de datos en un paso anterior, haga clic de nuevo en **Agregar servicio** y elija **Experiencia de Adobe[!DNL Platform]** en el campo desplegable. En el campo Conjunto de datos de evento, seleccione el conjunto de datos que ha creado anteriormente.
   * Guarde la secuencia de datos.

1. Por último, para ver los datos de [!DNL Commerce], deberá navegar a Analysis Workspace en el Adobe [!DNL Analytics], crear un proyecto, elegir el grupo de informes y agregar tablas de forma libre y otras visualizaciones para informar y analizar los datos de [!DNL Commerce]. La siguiente imagen muestra un ejemplo de una tabla que puede crear en Analysis Workspace.

   ![[!DNL Analytics] captura de pantalla de algunos datos de comercio](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Estos son algunos recursos adicionales para ayudarle a trabajar en Analysis Workspace:

   * [Información general de Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Generando un proyecto de Workspace desde cero](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Uso de tablas, visualizaciones y paneles en Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Casos de uso de visualización](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Además, hay cursos gratuitos disponibles en Experience League. Ver [!DNL Analytics] cursos disponibles [AQUÍ](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
