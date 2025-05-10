---
title: Integrar Adobe [!DNL Analytics] y Recorrido del cliente [!DNL Analytics] con el tutorial de Experience [!DNL Platform] Edge
description: Aprenda a integrar Adobe [!DNL Analytics] con el Recorrido del cliente [!DNL Analytics] mediante el SDK web de AEP, el SDK móvil de AEP o la API de servidor de Edge Network.
solution: Customer Journey [!DNL Analytics], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 3%

---

# Integrar el Adobe [!DNL Analytics] y el Recorrido del cliente [!DNL Analytics] con el tutorial de Edge de Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/es?lang=es#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crear esquemas</a> para la ingesta de datos.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear conjuntos de datos</a> para la ingesta de datos.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Configure las identidades y áreas de nombres de identidad correctas en el esquema</a> para asegurarse de que los datos ingeridos puedan vincularse a un perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=es" _target="_blank" rel="noopener noreferrer">Habilite los esquemas y conjuntos de datos para el perfil</a>.</li>
    <li>Ingresar datos en la experiencia [!DNL Platform] mediante uno de estos métodos:</li>
        <ul>
            <li>SDK web de Experience [!DNL Platform]:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul>
            <li>SDK para móviles de Experience [!DNL Platform]:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul></li>
            <li>API de Edge Network Server:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                </ul>
       </ul>
    <li><i>(Opcional)</i>. Si usa varios conjuntos de datos, vincule el ID de la persona para <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=es" _target="_blank" rel="noopener noreferrer">generar un conjunto de datos combinado</a>. Si utiliza un solo conjunto de datos de [!DNL Analytics] o si existe un identificador común en todos los conjuntos de datos que planea usar en el Recorrido del cliente [!DNL Analytics], omita este paso.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear una conexión</a> en el Recorrido del cliente [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear una vista de datos</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=es" _target="_blank" rel="noopener noreferrer">establecer la configuración del componente</a> y <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=es" _target="_blank" rel="noopener noreferrer">aplicar formato a las métricas</a> en el Recorrido del cliente [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=es" _target="_blank" rel="noopener noreferrer">Cree un proyecto en el Recorrido del cliente [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Los pasos estándar del flujo de trabajo para el conector de origen del Adobe [!DNL Analytics] crean el esquema y el conjunto de datos utilizados para ingerir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
