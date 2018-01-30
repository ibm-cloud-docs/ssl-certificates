---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualización y actualización de certificados SSL

Una vez que se haya importado un certificado SSL a la pantalla de certificados SSL, podrá verlo y actualizarlo en cualquier momento. Las actualizaciones funcionan de forma similar al [proceso de importación](import-ssl-certificate.html), ya que todos los detalles que se actualizan deben coincidir exactamente con los certificados originales, incluidos los espacios y los saltos de línea.

Para ver y actualizar un certificado SSL, lleve a cabo los pasos siguientes.

1. Acceda a [{{site.data.keyword.slportal_full}} ![icono de enlace externo](../../icons/launch-glyph.svg "icono de enlace externo")](https://control.softlayer.com/){: new_window} mediante sus credenciales únicas.
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
2. Seleccione **Ver/actualizar certificado** en la lista desplegable **Acciones**.
3. Actualice los **detalles del certificado SSL** en los recuadros de texto aplicables.

   **Nota:** Los detalles introducidos en la ventana **Importar certificado SSL** deben introducirse exactamente tal como los proporciona la autoridad de certificado, incluidos los espacios y los saltos de líneas. De lo contrario, se produce un error.

| Recuadro de texto | Entrada |
| -------- | ----- |
|Certificado |Detalles de certificado SSL, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Clave privada | Detalles de Clave privada del certificado, proporcionados por la autoridad de certificado. Generalmente, se trata de un bloque de texto alfanumérico.|
|Certificado intermedio | Detalles de certificado intermedio, proporcionados por la autoridad de certificado. Los certificados intermedios no son necesarios. Sin embargo, si la información está disponible para el certificado SSL, debe introducirse..|
| Solicitud de firma de certificado | Detalles de Solicitud de firma de certificado (CSR), proporcionados por la autoridad de certificado. No son necesarios los detalles de CSR, pero deben proporcionarse si son parte del certificado. **Nota:** no modifique el CSR de ninguna forma. Debe incluirse una clave pública con el CSR y no debería reemplazarse por la Clave privada.|
|Notas | Cualquier nota relacionada con el certificado SSL que pueda ser útil para otros usuarios.
Pulse **Actualizar** para actualizar el certificado SSL o bien en **Cancelar** para cancelar la acción.

## Pasos siguientes

Después de actualizar los detalles del certificado SSL, los productos y servicios que utilizan los certificados no tendrán una afectación negativa tras los cambios. Los certificados pueden volverse a actualizar en cualquier momento repitiendo los pasos anteriores.
