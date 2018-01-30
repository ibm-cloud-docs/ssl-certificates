---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-30"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introducción a los certificados SSL  


## Antes de empezar

Iniciarse en SSL requiere algo de planificación. Lleve a cabo los siguientes requisitos previos.

1. Decida de dónde obtener el certificado
2. Obtenga información sobre los tipos de certificados, la longitud de las claves y la duración
3. Seleccione un nombre común
4. Obtenga información sobre la regla de sockets
5. Genere el CSR

Para obtener más información, consulte [Planificación para certificados SSL](planning-ahead-ssl.html).

## Solicitud de certificados SSL

1. Acceda a [{{site.data.keyword.slportal}} ![icono de enlace externo](../../icons/launch-glyph.svg "icono de enlace externo")](https://control.softlayer.com/){: new_window} mediante sus credenciales únicas.
2. Seleccione **Seguridad > certificados SSL >** para acceder a la pantalla de certificados SSL.
3. Debe seleccionar el tipo de certificado y su duración, enviar el texto del CSR, rellenar algunos detalles adicionales y confirmar el pago.

## Instalación y pruebas
Una vez que se complete el proceso de solicitud y validación, recibirá un correo electrónico de la autoridad de certificado que incluye su certificado, así como cualquier certificado intermedio necesario. Su método de instalación dependerá del software que utilice, pero el resultado final debería ser el mismo. Cuando finalice, debería poder visitar <http://host.yourdomain.com> y ver tanto su contenido como el candado SSL que los navegadores utilizan para indicar que la sesión está cifrada. Si recibe una advertencia, debe llevar a cabo algunos pasos.

## Pasos siguientes

Después de que las pruebas sean correctas, puede acceder a la pantalla de certificados SSL, para [actualizar](view-and-update-ssl-certificate.html), [descargar](download-ssl-certificate-details.html), [suprimir](delete-ssl-certificate.html), o [importar](import-ssl-certificate.html) certificados SSL existentes a la herramienta.
