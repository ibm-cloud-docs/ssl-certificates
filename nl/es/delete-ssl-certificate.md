---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Supresión de certificados SSL
{: #deleting-ssl-certificates}

Una vez que se importan los detalles del certificado SSL en la consola de {{site.data.keyword.cloud}}, este puede suprimirse en cualquier momento para evitar que los datos se guarden en la consola de {{site.data.keyword.cloud_notm}}.

Para suprimir un certificado SSL, lleve a cabo los pasos siguientes.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Certificados**.
3. En el menú **Acciones**, seleccione **Suprimir** para el certificado SSL deseado.
4. Pulse **Sí** para suprimir el certificado SSL.

## Siguientes pasos

Tras suprimir un certificado SSL, todos los servicios relacionados con el certificado ya no utilizan su información. El certificado ya no aparece en la pantalla de certificados SSL de la consola de {{site.data.keyword.cloud_notm}}.

Actualice todos los servicios que previamente utilizaban el certificado asociándolos con un certificado SSL válido asociado con la cuenta.

En cualquier momento, el certificado SSL se puede volver a añadir a la consola de {{site.data.keyword.cloud_notm}} mediante el proceso de [importación](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates).
{:note}
