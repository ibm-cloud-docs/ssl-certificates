---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importación de certificados SSL
{: #importing-ssl-certificates}

Una vez que se emite un certificado SSL para un sitio web, puede importarse en la consola de {{site.data.keyword.cloud}}. Al importar certificados SSL en la consola de {{site.data.keyword.cloud_notm}}, dichos certificados pueden aplicarse a productos y servicios que puedan requerirlos, como la [Descarga SSL](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer) del Equilibrador de carga. De forma predeterminada, los certificados SSL emitidos por {{site.data.keyword.cloud_notm}} no se importan a la lista, ya que están pensados para que solo los manipule el destinatario. Así pues, un usuario autorizado de la cuenta debe importar los certificados SSL que se utilicen con un producto o servicio de {{site.data.keyword.cloud_notm}}.
{:shortdesc}

## Importación de certificados SSL

Complete los pasos siguientes para importar un certificado SSL.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. Pulse **Importar certificado SSL**.
4. Especifique los **detalles del certificado SSL** en los campos relevantes y pulse **Importar**. Consulte la tabla siguiente para obtener más información.

   Los detalles que se introducen en la ventana **Importar certificado SSL** deben introducirse exactamente tal como los proporciona la autoridad de certificado, incluidos los espacios y los saltos de líneas. De lo contrario, se produce un error.
   {:note}

| Detalles del certificado SSL     | Descripción |
| --------------------------- | ----------- |
|Certificado                  | Detalles de certificado SSL, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Clave privada                  | Detalles de clave privada del certificado, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Certificado intermedio     | Detalles de certificado intermedio, proporcionados por la autoridad de certificado. Los certificados intermedios no son necesarios; sin embargo, si la información está disponible para el certificado SSL, debe especificarse.|
|Solicitud de firma de certificado  | Detalles de solicitud de firma de certificado (CSR) proporcionados por la autoridad de certificado. No son necesarios los detalles de CSR, pero deben proporcionarse si son parte del certificado. **Nota:** no modifique la CSR de ninguna forma. Puede incluirse una clave pública con la CSR y no debería reemplazarse por la Clave privada.|
|Notas                        | Cualquier nota relacionada con el certificado SSL que pueda ser útil para otros usuarios.|
{: caption="Tabla 1. Detalles del certificado SSL" caption-side="top"}

## Siguientes pasos

Una vez que se ha importado el certificado SSL en la consola de {{site.data.keyword.cloud_notm}}, se almacena en la pantalla de certificados SSL hasta que se [suprima manualmente](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). Para los productos o servicios que requieran los detalles del certificado SSL, el nuevo certificado SSL aparece en la lista de certificados disponibles para utilizarlo al interactuar con la característica SSL para el producto o servicio deseado. El certificado puede [actualizarse](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) y los detalles del certificado pueden [descargarse de forma segura](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) en cualquier momento.
