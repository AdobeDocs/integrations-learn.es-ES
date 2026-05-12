---
title: Integrar Adobe [!DNL Analytics] y el Recorrido del cliente [!DNL Analytics] con el tutorial de Experience [!DNL Platform] Edge
description: Aprenda a integrar Adobe [!DNL Analytics] con el Recorrido del cliente [!DNL Analytics] mediante AEP Web SDK, AEP Mobile SDK o la API de servidor de Edge Network.
solution: Customer Journey Analytics, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integración" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
TQID: https://experienceleague.adobe.com/ClZddWXeWp51gWTBjRDQBZ2xNiO1bTRq-AoAdmucNEg
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
  - id: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
  - id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5e
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 413
ht-degree: 16%

---

# Integrar Adobe [!DNL Analytics] y el Recorrido del cliente [!DNL Analytics] con el tutorial de Edge de Experience [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/es?lang=es#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crear esquemas</a> para la ingesta de datos.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear conjuntos de datos</a> para la ingesta de datos.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Configure las identidades y áreas de nombres de identidad correctas en el esquema</a> para asegurarse de que los datos ingeridos puedan vincularse a un perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=es" _target="_blank" rel="noopener noreferrer">Habilite los esquemas y conjuntos de datos para el perfil</a>.</li>
    <li>Ingresar datos en la experiencia [!DNL Platform] mediante uno de estos métodos:</li>
        <ul>
            <li>Experiencia [!DNL Platform] Web SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul>
            <li>Experience [!DNL Platform] Mobile SDK:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html?lang=es" _target="_blank" rel="noopener noreferrer">Tutorial</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html?lang=es" _target="_blank" rel="noopener noreferrer">Lista de comprobación</a></li>
                </ul></li>
            <li>API de servidor de Edge Network:</li>
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
>Los pasos estándar del flujo de trabajo para el conector de origen de Adobe [!DNL Analytics] crean el esquema y el conjunto de datos utilizados para ingerir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
