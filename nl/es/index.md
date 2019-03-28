---

copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Guía de aprendizaje de iniciación
{: #getting-started-tutorial}


## Antes de empezar

Iniciarse en SSL requiere algo de planificación. Lleve a cabo los siguientes requisitos previos.

1. Decida de dónde obtener el certificado
2. Obtenga información sobre los tipos de certificados, la longitud de las claves y la duración
3. Seleccione un nombre común
4. Obtenga información sobre la regla de sockets
5. Genere el CSR

Para obtener más información, consulte [Planificación para certificados SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl).

## Solicitud de certificados SSL

1. Acceda al [{{site.data.keyword.slportal_full}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window} utilizando sus credenciales exclusivas.
2. Seleccione **Seguridad > certificados SSL >** para acceder a la pantalla de certificados SSL.
3. Debe seleccionar el tipo de certificado y su duración, enviar el texto del CSR, especificar algunos detalles adicionales y confirmar el pago.

## Instalación y pruebas
Una vez completado el proceso de solicitud y validación, recibirá un correo electrónico de la autoridad de certificado que incluye su certificado, así como cualquier certificado intermedio necesario. El método de instalación depende del software que utilice, pero el resultado final debería ser el mismo. Cuando finalice, debería poder navegar a <http://host.yourdomain.com> y ver tanto su contenido como el candado SSL que los navegadores utilizan para indicar que la sesión está cifrada. Si recibe una advertencia, debe llevar a cabo algunos pasos.

## Pasos siguientes

Después de que las pruebas sean correctas, puede acceder a la pantalla de certificados SSL, para [actualizar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates), [descargar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details), [suprimir](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates), o [importar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) certificados SSL existentes a la herramienta.
