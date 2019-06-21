---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Descarga de los detalles del certificado SSL
{: #downloading-ssl-certificate-details}

Una vez que se ha añadido el certificado SSL en la consola de {{site.data.keyword.cloud}}, pueden descargarse los detalles en cualquier momento. Las descargas pueden incluir el certificado, la clave o el PEM, que incluyen todos los detalles disponibles asociados con el certificado SSL. Los detalles del certificado SSL se descargan de forma segura, por lo que no hay ningún riesgo asociado con la recuperación de los detalles mediante este método.
{:shortdesc}

Para descargar los detalles del certificado SSL, lleve a cabo los pasos siguientes.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. En el menú **Acciones**, seleccione la **Opción de descarga** preferida para el certificado. Consulte la tabla siguiente para obtener más información:

| Opción de descarga      | Información descargada |
| -------------------- | -------------------- |
| Descargar certificado | Solo descarga la parte del certificado y no incluye la clave privada, el certificado intermedio, la solicitud de firma de certificado ni los detalles de las notas. |
| Descargar clave         | Solo descarga la clave privada y no incluye el certificado, el certificado intermedio, la solicitud de firma de certificado ni los detalles de las notas. |
| Descargar PEM         | Descarga todos los detalles asociados con el certificado SSL, incluido el certificado, la clave privada, el certificado intermedio, la solicitud de firma de certificado y las notas. |
{: caption="Tabla 1. Opciones de descarga" caption-side="top"}

## Siguientes pasos

Tras solicitar los detalles del certificado SSL para descargar, estos se descargan automáticamente en el navegador web. Seleccione la descarga para abrir el archivo. También se puede guardar el archivo en la estación de trabajo como referencia; sin embargo, se pueden descargar automáticamente los datos de cualquier certificado SSL presente en cualquier momento repitiendo los pasos anteriores.

