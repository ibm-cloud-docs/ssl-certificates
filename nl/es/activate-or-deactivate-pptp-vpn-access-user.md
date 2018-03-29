---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Activación o desactivación del acceso VPN de PPTP

La VPN de PPTP permite a los usuarios formar un túnel seguro a la red privada de {{site.data.keyword.BluSoftlayer_full}} mediante software especializado de cliente que se ejecuta en su sistema de escritorio o su dispositivo dedicado. El acceso PPTP se ha diseñado para clientes que necesiten conectar una oficina entera o que no puedan utilizar la solución VPN de SSL. Se asigna a cada cliente una conexión PPTP con conexiones adicionales disponibles, pero solicitando soporte para habilitar acceso ilimitado a PPTP, disponible sin coste adicional. Para activar o desactivar el acceso VPN de PPTP de un usuario, lleve a cabo los pasos siguientes.

1. Acceda al [{{site.data.keyword.slportal_full}} ![Icono de enlace externo](../../icons/launch-glyph.svg "Icono de enlace externo")](https://control.softlayer.com/){: new_window} utilizando sus credenciales exclusivas como administrador.
2. Localice el usuario cuyo acceso desee modificar y consulte la columna **Acceso VPN** para ver su nivel de acceso actual.
3. En el menú **Acciones**, seleccione **Editar acceso VPN**.
4. Especifique el tipo de VPN y los detalles de acceso de subred.

|Nombre de campo  |Opciones   |
| -----------| ------------ |
| Tipo de VPN   | Ninguno, SSL, PPTP o ambos (SSL y PPTP) |
|Acceso de subred | Automático o manual |           
{: caption="Tabla 1. Editar las opciones de acceso VPN" caption-side="top"}   
5. Pulse **Guardar** para guardar los cambios.

   **Nota:** debe activarse el acceso PPTP para que un usuario pueda conectarse mediante PPTP.
