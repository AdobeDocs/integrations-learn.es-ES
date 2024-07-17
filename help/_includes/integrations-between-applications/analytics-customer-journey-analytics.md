---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# Integrar el Adobe [!DNL Analytics] con el Recorrido del cliente [!DNL Analytics]

{{analytics-description}}

{{customer-journey-analytics-description}}

La integración del Adobe [!DNL Analytics] con el Recorrido del cliente [!DNL Analytics] ofrece ventajas clave:

+ **Información exhaustiva** sobre los comportamientos y preferencias de los clientes.
+ **Seguimiento en canales múltiples sin fisuras** para obtener una vista integral.
+ **Datos unificados e informes** para un análisis preciso.
+ **Personalización mejorada** y participación mejorada del cliente.
+ **Datos en tiempo real** para una toma de decisiones ágil.

## Integraciones comunes

<table>
    <thead>
        <tr>
            <th>aplicaciones de Experience Cloud</th>
            <th>Se integra mediante</th>
            <th>Cuándo usar</th>
            <th>Casos de uso comunes</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td rowspan="2">[!DNL Analytics] y Recorrido del cliente [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Conector de origen de Experience [!DNL Platform]</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Enfoque recomendado para los clientes que ya han implementado el Adobe [!DNL Analytics] y desean la forma más rápida de introducir estos datos en la experiencia [!DNL Platform] para usarlos en el Recorrido del cliente [!DNL Analytics].</li>
                    <li>Cuando la disponibilidad de los datos para el perfil del cliente puede estar entre 2 y 30 minutos desde el momento de la recopilación de datos, y la disponibilidad para el lago de datos es de hasta 90 minutos.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Flujo de trabajo iniciado directamente por la interfaz de usuario.</li>
                    <li>Asignando la interfaz de usuario para copiar [!DNL Analytics] props y eVars en nuevos campos XDM.</li>
                    <li>La forma más rápida de obtener valor de Perfil del cliente en tiempo real y Recorrido del cliente [!DNL Analytics].</li>
                </ul>
            </td>
        </tr>
        <tr>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">Experiencia [!DNL Platform] en Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Enfoque recomendado para nuevas implementaciones de [!DNL Analytics] o cuando se desea implementar una estrategia a largo plazo.</li>
                    <li>Envía datos directamente desde un dispositivo a Experience [!DNL Platform] mediante el SDK web de AEP, el SDK móvil de AEP o la API de servidor de Edge Network.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Proporciona el mayor nivel de control sobre los datos recopilados para ayudar en sus casos de uso.</li>
                    <li>Los datos del lado del cliente se asignan fácilmente a campos XDM.</li>
                    <li>La disponibilidad de datos más rápida para el Perfil del cliente en tiempo real.</li>
                </ul>
            </td>
        </tr>  
    </tbody>          
</table>
