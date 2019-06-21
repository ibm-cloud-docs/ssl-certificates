---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Activación o desactivación del acceso VPN de PPTP
{: #activating-or-deactivating-pptp-vpn-access}

La VPN de PPTP le permite formar un túnel seguro a la red privada de {{site.data.keyword.cloud}} mediante software especializado de cliente que se ejecuta en su sistema de escritorio o su dispositivo dedicado. El acceso PPTP se ha pensado como solución por si necesita conectar una oficina entera o no puede utilizar la solución VPN de SSL. Se le asigna una conexión PPTP con más conexiones disponibles y puede solicitar soporte para habilitar el acceso ilimitado a PPTP, disponible sin coste adicional. Para activar o desactivar el acceso VPN de PPTP de un usuario, lleve a cabo los pasos siguientes.
{:shortdesc}

1. Inicie una sesión en la página [Acceso (IAM)](https://cloud.ibm.com/iam/overview){: external} en la consola de {{site.data.keyword.cloud_notm}}.
2. Localice el usuario cuyo acceso desee modificar y consulte la columna **Acceso VPN** para ver su nivel de acceso actual.
3. En el menú **Acciones**, seleccione **Editar acceso VPN**.
4. Especifique el tipo de VPN y los detalles de acceso a la subred y pulse **Guardar** para guardar los cambios. Consulte la tabla siguiente para obtener más información.

|Nombre de campo  |Opciones   |
| -----------| ------------ |
| Tipo de VPN   | Ninguno, SSL, PPTP o ambos (SSL y PPTP) |
| Acceso de subred | Automático o manual |           
{: caption="Tabla 1. VPN y detalles de subred" caption-side="top"}   

Debe activarse el acceso PPTP para que un usuario pueda conectarse mediante PPTP.
{:note}
