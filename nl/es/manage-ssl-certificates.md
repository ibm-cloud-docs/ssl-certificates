---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gestión de certificados SSL

{{site.data.keyword.BluSoftlayer_full}} ahora proporciona una forma de almacenar certificados dentro de su portal. No solo puede servir como repositorio para gestionar sus certificados, sino que también es necesario si se utilizan servicio que pueden emplear certificados o que los requieran.

1. Acceda a [{{site.data.keyword.slportal_full}} ![icono de enlace externo](../../icons/launch-glyph.svg "icono de enlace externo")](https://control.softlayer.com/){: new_window} mediante sus credenciales únicas.
2. En el menú **Seguridad**, seleccione **SSL > Certificados > Gestionar certificados**.

Se le presenta una lista de sus certificados actuales, junto con información sobre su estado.

Puede buscar, descargar y descargar partes de un certificado o una versión PEM formateada, o bien revisar la caducidad de sus certificados. También puede ver cuántos servicios utilizan en ese momento cada certificado. Esto le permite saber si deben llevarse a cabo alguna acción cuando un certificado está a punto de caducar.

## Cómo añadir un certificado

Cuando esté listo para añadir un certificado, seleccione "Añadir certificado" en el menú de subnavegación o en el título de lista de certificados. Solo se le requiere que proporcione el certificado y clave privada de este. Sin embargo, no proporcionar un certificado intermedio si su emisor lo proporciona conlleva romper la cadena de certificado y una validación inadecuada de los usuarios finales o los servicios asociados.

Nota: no se pueden almacenar las claves privadas que requieren una contraseña.

Una vez añadido, los campos siguientes se derivan directamente de sus certificados:

* Nombre común
* Nombre de la organización
* Período de validez


¡Y ya está!

## Edición de un certificado

Al activar el triángulo de la izquierda de un certificado, se abrirán todas sus partes. Esto permite editar las partes del certificado. Debe añadirse una nota y, cuando sea necesario, debe eliminarse el certificado. También hay una lista de los servicios que actualmente utilizan el certificado.



Nota importante: solo los certificados que no están asociados con los servicios deben tener actualizadas las partes "clave privada", "certificado" o "certificado intermedio". El certificado no puede eliminarse.

Puede modificar la nota en cualquier momento.

## Eliminación de un certificado

Para eliminar un certificado, siga los pasos para editarlo y seleccionar el recuadro de selección "Confirmar eliminación de certificado" y guardar.

### API

La posibilidad de añadir, eliminar, editar y buscar sus certificados también está disponible mediante SLAPI sldn.softlayer.com. Se han proporcionado algunos ejemplos en artículo SLDN, sldn.softlayer.com/article/SSL-Management-my-SLAPI-Its-more-likely-you-think.
