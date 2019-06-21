---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renovación de certificados SSL
{: #renewing-ssl-certificates}

Una vez que se ha solicitado un certificado SSL mediante {{site.data.keyword.cloud}}, puede renovarse en cualquier momento. Durante el proceso de renovación, {{site.data.keyword.cloud_notm}} actúa como facilitador entre usted y la entidad emisora de certificados y no ve ni controla ninguna parte del proceso de renovación que implica los detalles del certificado SSL. Los certificados SSL se renuevan bajo los mismos términos en los que se solicitaron, por lo que no deben hacerse cambios en los detalles de renovación (tipo y autoridad de certificado, mes de validez, plataforma de servicio, etc.) Los certificados pueden renovarse antes o después de que hayan caducado; sin embargo, para mantener la validez del certificado SSL, renuévelo antes de su fecha de caducidad.
{:shortdesc}

## Renovación de un certificado SSL
Lleve a cabo los pasos siguientes para renovar un certificado SSL.

1. Vaya al menú de seguridad de la consola. Para obtener más información, consulte [Navegación a dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. En el menú **Seguridad**, seleccione **SSL > Pedidos**.
3. Pulse **Renovar** en la columna **Renovar** del certificado SSL deseado.
4. Determine si todos los detalles de CSR y de renovación son correctos antes de renovar el certificado SSL. Consulte la tabla siguiente para obtener más información.  

| Detalles                         | Acción  |
| ------------------------------- | ------- |
| Detalles de CSR y de renovación correctos | Seleccione **Renovar** para renovar el certificado SSL. |
| Detalles de renovación incorrectos       | Seleccione **Adquirir un nuevo certificado SSL** para solicitar un nuevo certificado. Dado que los detalles de renovación, incluidos el tipo, la autorización y el correo electrónico de aprobación del certificado no se pueden cambiar, la única manera de actualizar los detalles de un certificado SSL del sitio web es solicitar un certificado nuevo. |
| Detalles de CSR incorrectos           | Seleccione **Cambiar CSR**, especifique los nuevos detalles de CSR en el **recuadro de texto CSR** y seleccione **Restaurar CSR**. |
{: caption="Tabla 1. Detalles de renovación y de CSR" caption-side="top"}

## Siguientes pasos

Tras solicitar la renovación de un certificado SSL, {{site.data.keyword.cloud_notm}} reenvía la solicitud a la autoridad de certificado para finalizar la verificación del sitio web requerida para la renovación. Una vez que se renueva el certificado, en el campo **Caduca** aparece la nueva fecha de caducidad.
