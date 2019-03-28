---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renovación de certificados SSL
{: #renewing-ssl-certificates}

Una vez que se ha solicitado un certificado SSL mediante {{site.data.keyword.BluSoftlayer_full}}, puede renovarse en cualquier momento. Durante el proceso de renovación, {{site.data.keyword.BluSoftlayer_notm}} actúa como facilitador entre el cliente (usted) y la autoridad de certificado y no ve ni controla ninguna parte del proceso de renovación que implica los detalles del certificado SSL. Los certificados SSL se renuevan bajo los mismos términos en los que se solicitaron, por lo que no deben hacerse cambios en los Detalles de renovación (tipo y autoridad de certificado, mes de validez, plataforma de servicio, etc.) Los certificados pueden renovarse antes o después de que hayan caducado; sin embargo, para mantener la validez del certificado SSL, renuévelo antes de su fecha de caducidad. Lleve a cabo los pasos siguientes para renovar un certificado SSL.

## Renovación de un certificado SSL

1. Acceda al [{{site.data.keyword.slportal_full}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window} utilizando sus credenciales exclusivas.
2. En el menú **Seguridad**, seleccione **SSL > Pedidos**.
3. Pulse el enlace **Renovar** en la columna **Renovar** del certificado SSL deseado.

   **Nota:** Aparecerá un recuadro emergente para completar la solicitud.  
   * Determine si todos los detalles de CSR y de Renovación son correctos:<br /><br /><table border="1"><caption>Tabla 1. Detalles de renovación y de CSR</caption><tr><th>Si...</th><th>Entonces...</th></tr><tr><td>Todos los detalles de Renovación y CSR son correctos</td><td>Vaya al siguiente paso.</td></tr><tr><td>Los detalles de renovación no son correctos</td><td><ul><li>Pulse el enlace <strong>Adquirir un nuevo certificado SSL</strong> para que se le redirija a la pantalla de compra.<br /><blockquote><strong>Nota:</strong> Dado que los detalles de renovación, incluidos el tipo, la autorización y el correo electrónico de aprobación de certificado no se pueden cambiar, la única manera de actualizar los detalles de un certificado SSL del sitio web es solicitar un certificado nuevo.</blockquote></li><li>Complete las pantallas de la página de pedido con la información para el certificado SSL. No se requiere ninguna acción adicional con este procedimiento.</li></ul></td></tr><tr><td>Los detalles de CSR no son correctos</td><td><ul><li>Pulse el botón **Cambiar CSR**.</li><li>Especifique los **detalles de CSR nuevos** en el recuadro de texto **CSR**.</li><li>Pulse el botón **Restaurar CSR**.</li></ul></td></tr></table>
4. Pulse el botón **Renovar** para renovar el certificado SSL o pulse **Cancelar** para cancelar la acción.

## Pasos siguientes

Tras solicitar la renovación de un certificado SSL, {{site.data.keyword.BluSoftlayer_notm}} reenvía la solicitud a la autoridad de certificado para finalizar la verificación del sitio web requerida para la renovación. Una vez que se renueva el certificado, en el campo Caduca aparece la nueva fecha de caducidad.
