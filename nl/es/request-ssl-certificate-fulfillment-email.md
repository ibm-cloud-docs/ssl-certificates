---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Solicitud de un correo electrónico de tramitación del certificado SSL

## Visión general

Tras solicitar un nuevo certificado SSL mediante {{site.data.keyword.BluSoftlayer_full}}, la autoridad de certificado envía un correo electrónico de tramitación al administrador de dominio proporcionado durante el proceso de solicitud. Este correo electrónico contiene todos los detalles asociados con el certificado SSL. El correo electrónico de tramitación puede volver a solicitarse en cualquier momento desde la pantalla Pedidos SSL en {{site.data.keyword.slportal_full}}. Lleve a cabo los pasos siguientes para solicitar el correo electrónico de tramitación de SSL desde la autoridad de certificado.

## Solicitud de un correo electrónico de tramitación

1. Acceda a [{{site.data.keyword.slportal_full}} ![icono de enlace externo](../../icons/launch-glyph.svg "icono de enlace externo")](https://control.softlayer.com/){: new_window} mediante sus credenciales únicas.
2. En el menú **Seguridad**, seleccione **SSL > Pedidos**.
3. Pulse el enlace **Enviar** en la columna **Correo electrónico** del certificado SSL deseado.<br/>**Nota:** aparece una ventana emergente para confirmar la solicitud. Esta ventana contiene la dirección de correo electrónico del Administrador de dominios proporcionado cuando se solicitó el certificado SSL.
4. Pulse el botón **Reenviar correo electrónico** para confirmar la selección y solicitar un correo electrónico de tramitación adicional de la autoridad de certificado. Pulse **Cancelar** para cancelar la acción.

## Qué sucede a continuación

Tras solicitar un correo electrónico de tramitación adicional, la solicitud se reenviará a la autoridad de certificado correspondiente para su finalización. Dado que los detalles del certificado SSL son confidenciales, {{site.data.keyword.BluSoftlayer_notm}} no almacena los datos del certificado SSL en nuestro sistema. Una vez reciban los detalles del certificado SSL por correo electrónico, pueden [importarse](import-ssl-certificate.html) manualmente al {{site.data.keyword.slportal}} si es necesario.
