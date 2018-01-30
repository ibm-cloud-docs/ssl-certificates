---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Supresión de certificados SSL

## Visión general

Una vez que se importan los detalles del certificado SSL en el {{site.data.keyword.slportal_full}}, este puede suprimirse en cualquier momento para evitar que los datos se guarden en {{site.data.keyword.slportal}}.

Para suprimir un certificado SSL, lleve a cabo los pasos siguientes.

## Supresión de un certificado SSL

1. Acceda a [{{site.data.keyword.slportal}} ![icono de enlace externo](../../icons/launch-glyph.svg "icono de enlace externo")](https://control.softlayer.com/){: new_window} mediante sus credenciales únicas.
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. En el menú **Acciones**, seleccione **Suprimir** para el certificado SSL deseado.

  **Nota:** aparece una ventana para confirmar la supresión.
4. Pulse **Sí** para suprimir el certificado SSL o pulse **No** para cancelar la acción.

## Pasos siguientes

Tras suprimir un certificado SSL, todos los servicios relacionados con el certificado ya no utilizarán su información. El certificado ya no aparece en la pantalla de certificados SSL en {{site.data.keyword.slportal}}.

Se recomienda que actualice todos los servicios que previamente utilizaban el certificado asociándolos con un certificado SSL válido asociado con la cuenta.

**Nota:** en cualquier momento, puede volver a añadirse el certificado SSL a {{site.data.keyword.slportal}} mediante el proceso de [importación](import-ssl-certificate.html).
