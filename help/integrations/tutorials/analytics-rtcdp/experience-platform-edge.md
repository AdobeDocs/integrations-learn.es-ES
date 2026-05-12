---
title: Integrar  [!DNL Analytics] datos de clientes en tiempo real y [!DNL Platform] con el tutorial de Experience [!DNL Platform] Edge
description: Aprenda a integrar Adobe [!DNL Analytics] con datos de clientes en tiempo real [!DNL Platform] mediante AEP Web SDK, AEP Mobile SDK o la API de servidor de Edge Network.
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="Integración" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
TQID: https://experienceleague.adobe.com/K1CpRtUekl5jQNDMGswJpexC9fv9uVmgraLlNFXUIr8
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
  - id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2:
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
source-wordcount: 317
ht-degree: 10%

---

# Integrar Adobe [!DNL Analytics] y los datos de clientes en tiempo real [!DNL Platform] con el tutorial de Edge de la experiencia [!DNL Platform]

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
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear segmentos en la experiencia [!DNL Platform].</a> El sistema determina automáticamente si el segmento se evalúa como por lotes (conector de datos) o por secuencias (red Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Configure destinos para compartir atributos de perfil y pertenencias de audiencias en los destinos deseados.</a></li>
</ol>

>[!NOTE]
>
>Los pasos estándar del flujo de trabajo para el conector de origen de Adobe [!DNL Analytics] crean el esquema y el conjunto de datos utilizados para ingerir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
