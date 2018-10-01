---
copyright:
  years: 2014, 2018
lastupdated: "2018-06-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importación de certificados SSL

Una vez que se emite un certificado SSL para un sitio web, puede importarse en el {{site.data.keyword.slportal_full}}. Al importar certificados SSL al {{site.data.keyword.slportal}}, dichos certificados pueden aplicarse a productos y servicios que puedan requerirlos, como la [Descarga SSL](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window} del Equilibrador de carga. De forma predeterminada, los certificados SSL emitidos por {{site.data.keyword.BluSoftlayer_full}} no se importan a la lista, ya que están pensados para que solo los manipule el destinatario. Así pues, un usuario autorizado de la cuenta debe importar los certificados SSL que se vayan a utilizar con un producto o servicio de {{site.data.keyword.BluSoftlayer_notm}}. Complete los pasos siguientes para importar un certificado SSL al {{site.data.keyword.slportal}}.

1. Acceda al [{{site.data.keyword.slportal_full}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window} utilizando sus credenciales exclusivas.
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. Pulse **Importar certificado SSL**.
4. Introduzca los **detalles del certificado SSL** en los campos relevantes y pulse **Importar**.

   **Nota:** Los detalles que se introducen en la ventana **Importar certificado SSL** deben introducirse exactamente tal como los proporciona la autoridad de certificado, incluidos los espacios y los saltos de líneas. De lo contrario, se produce un error.

| Detalles del certificado SSL     | Descripción |
| --------------------------- | ----------- |
|Certificado                  | Detalles de certificado SSL, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Clave privada                  | Detalles de Clave privada del certificado, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Certificado intermedio     | Detalles de certificado intermedio, proporcionados por la autoridad de certificado. Los certificados intermedios no son necesarios. Sin embargo, si la información está disponible para el certificado SSL, debe introducirse..|
|Solicitud de firma de certificado  | Detalles de Solicitud de firma de certificado (CSR), proporcionados por la autoridad de certificado. No son necesarios los detalles de CSR, pero deben proporcionarse si son parte del certificado. **Nota:** no modifique el CSR de ninguna forma. Puede incluirse una clave pública con el CSR y no debería reemplazarse por la Clave privada.|
|Notas                        | Cualquier nota relacionada con el certificado SSL que pueda ser útil para otros usuarios.|
{: caption="Tabla 1. Detalles del certificado SSL" caption-side="top"}

## Pasos siguientes

Una vez que se ha importado el certificado SSL al {{site.data.keyword.slportal}}, se almacena en la pantalla de certificados SSL hasta que se [suprima manualmente](delete-ssl-certificate.html). Para los productos o servicios que requieran los detalles del certificado SSL, el nuevo certificado SSL aparece en la lista de certificados disponibles para utilizarlo al interactuar con la característica SSL para el producto o servicio deseado. El certificado puede [actualizarse](view-and-update-ssl-certificate.html) y los detalles del certificado pueden [descargarse de forma segura](download-ssl-certificate-details.html) en cualquier momento.
