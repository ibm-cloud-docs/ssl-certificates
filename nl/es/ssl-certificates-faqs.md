---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

<a name="top"></a>
# Preguntas frecuentes: certificados SSL

## ¿Por qué no se muestra automáticamente el certificado SSL que he solicitado en la pantalla de certificados SSL?
{:faq}

Una autoridad de certificados de terceros emite los certificados SSL y le envía todos los detalles del certificado directamente en un correo electrónico confidencial. Una vez que haya recibido el correo electrónico, tiene la opción de [importar el certificado SSL](import-ssl-certificate.html) al {{site.data.keyword.slportal_full}} si decide utilizar el certificado con productos y servicios de {{site.data.keyword.BluSoftlayer_full}}. Como {{site.data.keyword.cloud_notm}} nunca recibe los detalles del certificado SSL, los datos no pueden importarse automáticamente.

## ¿Qué es un certificado SSL?
{:faq}

Los sitios web habilitan certificados SSL como medida de seguridad para proteger al usuario. Por lo general, se utilizan cuando se le requiere transmitir información confidencial a un sitio web, como el nombre, la dirección, los números de tarjeta de crédito y otros datos personales o están gestionando datos que requieren autenticación (por ejemplo, información dentro de nuestro sitio web {{site.data.keyword.slportal}}). La empresa que ejecuta el sitio web solicita certificados SSL, pero los emite una empresa de terceros de confianza que garantiza la validez del sitio web. Los sitios web seguros están precedidos por HTTPS en el URL, al contrario que el HTTP estándar.

## ¿Cómo puedo solicitar un SSL SHA2?
{:faq}

Si ya ha solicitado un SSL y muestra errores de que el certificado SSL utiliza SHA-1 en lugar de SHA-2, debe solicitar que se vuelva a emitir el SSL enviando una incidencia.

Si todavía no ha solicitado un SSL a {{site.data.keyword.cloud_notm}} y debe solicitar uno con SHA-2, envíe una incidencia para solicitar manualmente un SSL para el dominio en cuestión. {{site.data.keyword.slportal}} todavía crea automáticamente certificados SSL mediante SHA-1, de forma que, si lo hace, tendrá que solicitar su reemisión.
