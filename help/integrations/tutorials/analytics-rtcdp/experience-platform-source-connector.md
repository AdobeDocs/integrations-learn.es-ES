---
title: Integrar  [!DNL Analytics] y datos de clientes en tiempo real [!DNL Platform] con el tutorial del conector de origen Experience [!DNL Platform] y
description: Aprenda a integrar Adobe [!DNL Analytics] con datos de clientes en tiempo real [!DNL Platform] usando el conector de origen Experience [!DNL Platform] s.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integración" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 2%

---

# Integrar el Adobe [!DNL Analytics] y los datos de clientes en tiempo real [!DNL Platform] con el conector de origen de la experiencia [!DNL Platform]

<ol>
    <li><a href="https://experienceleague.adobe.com/es?lang=es#dashboard/learning" _target="_blank" rel="noopener noreferrer">Crear esquemas</a> para la ingesta de datos.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear conjuntos de datos</a> para la ingesta de datos.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Configure las identidades y áreas de nombres de identidad correctas en el esquema</a> para asegurarse de que los datos ingeridos puedan vincularse a un perfil unificado.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=es" _target="_blank" rel="noopener noreferrer">Habilite los esquemas y conjuntos de datos para el perfil</a>.</li>
    <li>Ingresar datos de [!DNL Analytics] en Experience Platform mediante el <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=es" _target="_blank" rel="noopener noreferrer">conector de origen del Adobe [!DNL Analytics]</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html?lang=es" _target="_blank" rel="noopener noreferrer">Crear segmentos en la experiencia [!DNL Platform].</a> El sistema determina automáticamente si el segmento se evalúa como por lotes (conector de datos) o como de flujo continuo (red Edge).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html?lang=es" _target="_blank" rel="noopener noreferrer">Configure destinos para compartir atributos de perfil y pertenencias de audiencias en los destinos deseados.</a></li>   
</ol>

>[!NOTE]
>
>Los pasos estándar del flujo de trabajo para el conector de origen del Adobe [!DNL Analytics] crean el esquema y el conjunto de datos utilizados para ingerir los datos de [!DNL Analytics] &quot;tal cual&quot;. Por lo tanto, el sistema gestiona los dos primeros pasos. El flujo de trabajo de asignación requiere la creación de atributos personalizados; por lo tanto, siga totalmente la secuencia de pasos.
