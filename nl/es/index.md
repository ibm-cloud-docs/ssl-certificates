---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

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
5. Genere la CSR

Para obtener más información, consulte [Planificación para certificados SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## Solicitud de certificados SSL

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **Seguridad > SSL > Certificados**.
3. Seleccione **Solicitar certificado SSL**.
3. Seleccione el tipo de certificado y su duración, envíe el texto de la CSR, seleccione la plataforma de servidor y luego confirme el pago.

## Instalación y pruebas
Una vez completado el proceso de solicitud y validación, recibirá un correo electrónico de la autoridad de certificado que incluye su certificado, así como cualquier certificado intermedio necesario. El método de instalación depende del software que utilice, pero el resultado final debería ser el mismo. Cuando finalice, debería poder navegar a `http://host.yourdomain.com` y ver tanto su contenido como el candado SSL que los navegadores utilizan para indicar que la sesión está cifrada. Si recibe una advertencia, debe llevar a cabo algunos pasos.

## Siguientes pasos

Después de realizar la prueba correctamente, puede acceder a sus certificados SSL en la consola de {{site.data.keyword.cloud_notm}} para [actualizar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [descargar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [suprimir](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) o [importar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) certificados SSL existentes en la herramienta.
