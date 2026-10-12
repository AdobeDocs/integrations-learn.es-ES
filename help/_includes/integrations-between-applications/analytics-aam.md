---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%
---

# Integración de [!DNL Analytics] y Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Al habilitar esta integración, al reenviar los datos del lado del servidor de Adobe [!DNL Analytics] a Audience Manager, Audience Manager obtiene una de sus principales fuentes de datos, a saber, los datos de comportamiento de los clientes en línea. Estos datos se pueden combinar con otros datos, como datos de CRM de origen o datos de socios de terceros, para crear segmentos de clientes enriquecidos. Además, los segmentos de Audience Manager se envían de vuelta a la página web en la respuesta de para un análisis más detallado del visitante. A continuación se describen ambos casos de uso importantes.

Las ventajas clave de integrar Adobe [!DNL Analytics] y Audience Manager son:

+ **Segmentación mejorada**: Combine los datos de Adobe [!DNL Analytics] y Audience Manager para obtener segmentos de audiencia precisos y personalizados en las campañas de marketing.
+ **Perfiles de cliente unificados**: integre fuentes de datos para comprender las interacciones y los comportamientos y cree perfiles de cliente completos.
+ **Mayor eficacia de la publicidad**: optimice la publicidad con direccionamiento basado en datos desde la integración de Adobe [!DNL Analytics] y Audience Manager.
+ **Decisiones basadas en datos**: Informe las opciones a través de información detallada, combinando datos de Adobe [!DNL Analytics] y Audience Manager.
+ **Experiencias personalizadas**: Adapte el contenido y las ofertas y enriquezca las interacciones de los clientes en distintos puntos de contacto mediante ambas plataformas.

En general, esta integración reúne datos valiosos y perspectivas de audiencia. Permite a las empresas crear campañas de marketing más específicas y relevantes, a la vez que logran un conocimiento más profundo de las preferencias y comportamientos de sus clientes.

## Integraciones comunes

<table>
    <thead>
        <tr>
            <th>Aplicaciones de Experience Cloud</th>
            <th>Se integra mediante</th>
            <th>Cuándo usar</th>
            <th>Casos de uso comunes</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] está enviando datos a Audience Manager</a>
            </td>
            <td>Extensión de etiquetas Adobe [!DNL Analytics] para AppMeasurement.js con reenvío del lado del servidor habilitado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Si desea enviar datos de Adobe [!DNL Analytics] a Audience Manager para crear segmentos que se puedan compartir con otros destinos de Adobe Experience Cloud, destinos basados en personas u otros destinos personalizados y basados en dispositivos compatibles con Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Comparta segmentos con plataformas de anuncios que incluyan atributos de comportamiento recopilados en [!DNL Analytics].</li>
                    <li>Enriquezca los segmentos con datos de [!DNL Analytics] para crear segmentos de alto valor en canales múltiples y usarlos en la segmentación en el sitio.</li>
                    <li>Capa de datos de [!DNL Analytics] en segmentos sin clave en identificadores hash, como correo electrónico, para usar en plataformas de medios sociales.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager devuelve datos a [!DNL Analytics]</a>
            </td>
            <td>Extensión de etiquetas Adobe [!DNL Analytics] para AppMeasurement.js con reenvío del lado del servidor habilitado</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Cuando quiera compartir segmentos de Audience Manager con [!DNL Analytics] para informar sobre la detección de audiencias, la segmentación y la optimización.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Use segmentos de Audience Manager que incluyan datos demográficos de proveedores de terceros en [!DNL Analytics] informes.</li>
                    <li>Use segmentos de Audience Manager que incluyan datos de campaña de servidores de publicidad en [!DNL Analytics] informes.</li>
                    <li>Use segmentos de Audience Manager que incluyan datos CRM incorporados en [!DNL Analytics] informes.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
