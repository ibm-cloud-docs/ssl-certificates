---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Solicitud de un correo electrónico de tramitación del certificado SSL
{: #requesting-an-ssl-certificate-fulfillment-email}

Tras solicitar un nuevo certificado SSL mediante {{site.data.keyword.cloud}}, la autoridad de certificado envía un correo electrónico de tramitación al administrador de dominio proporcionado durante el proceso de solicitud. Este correo electrónico contiene todos los detalles asociados con el certificado SSL. El correo electrónico de tramitación puede volver a solicitarse en cualquier momento desde la pantalla Pedidos SSL en la consola de {{site.data.keyword.cloud_notm}}.
{:shortdesc}

## Solicitud de un correo electrónico de tramitación
Lleve a cabo los pasos siguientes para solicitar el correo electrónico de tramitación de SSL desde la autoridad de certificado.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Pedidos**.
3. Pulse **Enviar** en la columna **Correo electrónico** del certificado SSL que desea.

  Aparece una ventana emergente para confirmar la solicitud. Esta ventana contiene la dirección de correo electrónico del administrador del dominio proporcionado cuando se solicitó el certificado SSL.
  {:note}

4. Pulse en **Reenviar correo electrónico** para confirmar la selección y solicitar un correo electrónico de tramitación adicional de la autoridad de certificado.

## Siguientes pasos

Tras solicitar un correo electrónico de tramitación adicional, la solicitud se reenviará a la autoridad de certificado correspondiente para su finalización. Dado que los detalles del certificado SSL son confidenciales, {{site.data.keyword.cloud_notm}} no almacena los datos del certificado SSL en el sistema. Una vez recibidos los detalles del certificado SSL por correo electrónico, puede [importarlos](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) manualmente en la consola de {{site.data.keyword.cloud_notm}} si es necesario.
