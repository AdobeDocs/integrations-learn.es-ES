---
title: Integraciones de aplicaciones para la personalización a escala
description: Haga que las experiencias personalizadas formen parte de cada momento.
exl-id: 6d18813d-950c-40ae-8d5b-80bf389358fc
source-git-commit: 509b227f360718e81fb19d3a4d30aebf9de49e5a
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---

# Personalización a escala

Dentro del panorama actual, altamente competitivo y basado en la digitalización, los clientes han llegado a esperar experiencias adaptadas a sus preferencias y necesidades únicas. El uso de las capacidades de Adobe Experience Cloud nos permite recopilar y analizar una gran cantidad de datos de clientes, lo que nos proporciona una valiosa perspectiva de los comportamientos, los intereses y las preferencias. Esta comprensión profunda facilita la entrega de experiencias personalizadas en varios puntos de contacto, lo que garantiza interacciones significativas y atractivas. El uso del poder de Adobe Experience Cloud desbloquea todo el potencial de la personalización, fomentando conexiones de clientes más sólidas, fomentando la lealtad e impulsando el crecimiento empresarial.

<table>
 <thead>
    <tr>
      <th>Caso de uso</th>
      <th>Descripción</th>
      <th>Ejemplos</th>
      <th>Aplicaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>Creación de documentos personalizados de PDF</strong></td>
      <td>
        Generar documentos de comunicación para firmar en función de las selecciones/preferencias del usuario.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Presentar un NDA generado dinámicamente basado en los datos de un envío de AEM Forms para su firma
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-acrobat-sign.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Forms y Sign</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Análisis de datos e informes</strong></td>
      <td>
        Analizar datos de comportamiento desde experiencias digitales <br />Usar Adobe
        [!DNL Analytics] datos de comportamiento en Analysis Workspace en Customer Recorrido
        [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Analizar rutas de conversión superior/inferior</li>
          <li>Analizar la participación y conversión del canal</li>
          <li>Comprender el contenido más visto</li>
          <li>Comprender las principales categorías y productos de productos</li>
          <li>
            Realizar un análisis del uso de las herramientas para optimizar las experiencias de autoservicio
          </li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] y Recorrido del cliente [!DNL Analytics]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Informes de actividades de personalización<br />Analizar los resultados de las pruebas de optimización, incluidas las pruebas A/B, utilizando el Adobe [!DNL Target] y generación de informes completos mediante el Adobe [!DNL Analytics].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Mostrar resultados de pruebas A/B en informes de análisis enriquecidos</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] y [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalización de entregas de correo electrónico</strong></td>
      <td>
        Personalice las entregas de correo electrónico con contenido dinámico aprovechando las capacidades del Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Adición de ofertas personalizadas a correos electrónicos del cliente</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/campaign//campaign-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Campaign] y [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2">
        <strong>Expandir audiencias para plataformas de personalización y publicidad</strong>
      </td>
      <td>
        Utilice segmentos de Audience Manager para crear audiencias en Real-Time CDP y utilizarlas en tácticas de personalización y remarketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Realizar la segmentación y personalización de audiencias digitales anónimas en el sitio web, la aplicación móvil o en canales de publicidad admitidos
          </li>
          <li>
            Optimizar las experiencias de página de aterrizaje y autenticación previa en función de las características de comportamiento y del dispositivo conocidas
          </li>
          <li>
            Aproveche la red de datos de terceros Audience Manager para refinar y expandir aún más sus audiencias de segmentación
          </li>
          <li>Uso compartido de segmentos del Audience Manager con RTCDP</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/aam/aam-rtcdp.md"
          target="_blank"
          rel="noopener noreferrer"
          >Audience Manager y datos de clientes en tiempo real [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Uso [!DNL Analytics] datos para crear audiencias que se utilizarán en tácticas de personalización o remarketing.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>
            Realice la segmentación y personalización de audiencias digitales en dispositivos o canales publicitarios admitidos.
          </li>
          <li>
            Optimizar las páginas de aterrizaje conocidas del cliente y las experiencias anónimas en función del dispositivo y los atributos de comportamiento.
          </li>
          <li>Active audiencias en canales conocidos, como correo electrónico y SMS.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/analytics/analytics-customer-journey-analytics.md"
          target="_blank"
          rel="noopener noreferrer"
          >[!DNL Analytics] y datos de clientes en tiempo real [!DNL Platform]</a
        >
      </td>
    </tr>
    <tr>
      <td rowspan="2"><strong>Personalización de experiencias web</strong></td>
      <td>
        SPA AEM Personalice las experiencias de aplicación de una sola página () utilizando de forma eficaz la tecnología sin encabezado junto con el Adobe [!DNL Target].
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>SPA Personalización de aplicaciones móviles y de</li>
          <li>Respuestas de API personalizadas.</li>
          <li>[!DNL Target]Envío de contenido finalizado.</li>
          <li>Variaciones de prueba A/B.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM Sin encabezado y [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td>
        Ofrezca experiencias de sitio web adaptadas mediante la utilización eficaz de AEM Sites y Adobe [!DNL Target] para personalización.
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>AEM Personalización del sitio web de.</li>
          <li>Personalice el contenido del sitio web.</li>
          <li>Optimizar experiencias de usuario.</li>
          <li>Variaciones de prueba A/B.</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/experience-manager/experience-manager-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >AEM SITES y [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Personalizar experiencias digitales</strong></td>
      <td>
        Utilice los perfiles de cliente en tiempo real y los informes administrados de forma centralizada [!DNL Platform] segmentos para personalizar la mensajería en canales web, móviles y otros canales digitales
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalización de contenido para visitantes conocidos</li>
          <li>Aumentar la inscripción y participación con fines de fidelidad</li>
          <li>Identificación y participación de clientes en riesgo de pérdida</li>
          <li>Personalización de ofertas en tiempo real</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Datos de clientes en tiempo real [!DNL Platform] y [!DNL Target]</a
        >
      </td>
    </tr>
    <tr>
      <td><strong>Mejorar la generación de posibles clientes</strong></td>
      <td>
        Utilice los perfiles de cliente en tiempo real y los informes administrados de forma centralizada [!DNL Platform] segmentos para personalizar la mensajería en canales web, móviles y otros canales digitales
      </td>
      <td>
        <ul style="margin-top: 0;">
          <li>Personalización de contenido para visitantes conocidos</li>
        </ul>
      </td>
      <td>
        <a
          href="../integrations-between-applications/rtcdp/rtcdp-target.md"
          target="_blank"
          rel="noopener noreferrer"
          >Datos de clientes en tiempo real [!DNL Platform] y [!DNL Target]</a
        >
      </td>
    </tr>
  </tbody>
</table>
