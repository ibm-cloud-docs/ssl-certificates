---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualización y actualización de certificados SSL
{: #viewing-and-updating-ssl-certificates}

Una vez que se ha importado un certificado SSL a la pantalla de certificados SSL, puede verlo y actualizarlo en cualquier momento. Las actualizaciones funcionan de forma similar al [proceso de importación](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates), ya que todos los detalles que se actualizan deben coincidir exactamente con los certificados originales, incluidos los espacios y los saltos de línea.
{:shortdesc}

Para ver y actualizar un certificado SSL, lleve a cabo los pasos siguientes.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. Seleccione **Ver/actualizar certificado** en la lista desplegable **Acciones**.
4. Actualice los **detalles del certificado SSL** en los recuadros de texto aplicables y pulse **Actualizar** para aplicar los cambios. Consulte la tabla siguiente para obtener más información.

   Los detalles que se introducen en la ventana **Importar certificado SSL** deben introducirse exactamente tal como los proporciona la autoridad de certificado, incluidos los espacios y los saltos de líneas. De lo contrario, se produce un error.
   {:note}

| Detalles del certificado SSL     | Descripción |
| --------------------------- | ----------- |
|Certificado                  | Detalles de certificado SSL proporcionados por la entidad emisora de certificados. Generalmente, se trata de un bloque de texto alfanumérico.|
|Clave privada                  | Detalles de Clave privada del certificado proporcionados por la entidad emisora de certificados. Generalmente, se trata de un bloque de texto alfanumérico.|
|Certificado intermedio     | Detalles del certificado intermedio proporcionados por la entidad emisora de certificados. Los certificados intermedios no son necesarios; sin embargo, si la información está disponible para el certificado SSL, debe especificarse.|
|Solicitud de firma de certificado  | Detalles de solicitud de firma de certificado (CSR) proporcionados por la autoridad de certificado. No son necesarios los detalles de CSR, pero deben proporcionarse si son parte del certificado. **Nota:** no modifique la CSR de ninguna forma. Puede incluirse una clave pública con la CSR y no debería reemplazarse por la clave privada.|
|Notas                        | Cualquier nota relacionada con el certificado SSL que pueda ser útil para otros usuarios.|
{: caption="Tabla 1. Detalles del certificado SSL" caption-side="top"}

## Siguientes pasos

Después de actualizar los detalles del certificado SSL, los productos y servicios que utilizan los certificados no tendrán una afectación negativa tras los cambios. El certificado puede volverse a actualizar en cualquier momento repitiendo los pasos anteriores.
