---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestión de certificados SSL

{{site.data.keyword.BluSoftlayer_full}} ahora proporciona una forma de almacenar certificados dentro de su portal. No solo puede servir como repositorio para gestionar sus certificados, sino que también es necesario si se utilizan servicio que pueden emplear certificados o que los requieran.

1. Acceda al [{{site.data.keyword.slportal_full}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window} utilizando sus credenciales exclusivas.
2. En el menú **Seguridad**, seleccione **SSL > Certificados > Gestionar certificados**.

Se le presenta una lista de sus certificados actuales, junto con información sobre su estado.

Puede buscar, descargar y descargar partes de un certificado o una versión PEM formateada, o bien revisar la caducidad de sus certificados. También puede ver cuántos servicios utilizan en ese momento cada certificado. Esto le permite saber si debe llevarse a cabo alguna acción cuando un certificado está a punto de caducar.

## Cómo añadir un certificado

Cuando esté listo para añadir un certificado, seleccione "Añadir certificado" en el menú de subnavegación o en el título Lista de certificados. Solo se le requiere que proporcione el certificado y clave privada de este. Sin embargo, no proporcionar un certificado intermedio si su emisor lo proporciona conlleva romper la cadena de certificado y una validación inadecuada de los usuarios o los servicios asociados.

Nota: no se pueden almacenar las claves privadas que requieren una contraseña.

Una vez añadido, los campos siguientes se derivan directamente de sus certificados:

* Nombre común
* Nombre de la organización
* Período de validez

## Edición de un certificado

Al activar el triángulo de la izquierda de un certificado se abren todas sus partes. Esto permite editar las partes del certificado. Puede añadirse una nota y, cuando sea necesario, puede eliminarse el certificado. También hay una lista de los servicios que actualmente utilizan el certificado.

**Nota**: Solo se pueden tener actualizadas las partes "clave privada", "certificado" o "certificado intermedio" de los certificados que no están asociados con los servicios. El certificado tampoco puede eliminarse.

Puede modificar la nota en cualquier momento.

## Eliminación de un certificado

Para eliminar un certificado, siga los pasos para editarlo, seleccione "Confirmar eliminación de certificado" y guárdelo.

### API

Para ver un ejemplo de edición de certificados mediante la API, consulte [Gestión de SSL ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](http://sldn.softlayer.com/article/ssl-management){: new_window}. 
