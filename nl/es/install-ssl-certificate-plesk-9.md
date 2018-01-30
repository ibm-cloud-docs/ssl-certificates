---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalación de certificados SSL en Plesk 9

Para añadir certificados SSL en Plesk 9, lleve a cabo los pasos siguientes.

1. Inicie sesión en Plesk y vaya al dominio en el que desee instalar el certificado.
2. Vaya a la configuración del dominio de destino.
3. Pulse **Certificados SSL**.
4. Pulse **Añadir certificado SSL**.

   **Nota:** si ya dispone de un certificado SSL, omita este paso y vaya al paso 8.
5.  Dé un nombre al certificado. Puede darle cualquier nombre, pero puede ser útil usar un nombre descriptivo, por ejemplo, una marca de hora.

   En este caso, utilizaremos el formato *AAAAMMDDRR*, donde *RR* es el número de revisión (en este case, 00, ya que no hay revisiones realizadas el mismo día).
6. Haga todos los ajustes necesarios a la solicitud SSL. Esta información se incluirá en el certificado SSL y debería ser parecida a la información de registro del dominio.

  La dirección de correo electrónico debería coincidir con una de las direcciones de correo electrónico en el dominio cuya información proporcionó el registrador de dominios.

  **Importante:** es posible que la autoridad de certificado SSL rechace información falsa.
7. Vuelva a la configuración de certificado.
8. Revise la clave CSR y la clave privada y guarde la clave privada en una ubicación segura.  

  **Nota:** si hay cualquier problema con el servidor y el certificado tiene que volver a introducirse, debe tener como mínimo el certificado y la clave privada.
9. Tome el CSR y envíelo a la Autoridad de certificado que elija. La infraestructura de {{site.data.keyword.cloud_notm}} no proporciona certificados SSL.
10. Una vez que haya recibido el certificado de su Autoridad de certificado, puede pegarlo en el área de texto del certificado.

   **Notas:**
   * Si su Autoridad de certificado lo requiere, es posible que deba pegar su propio certificado en el área de texto del certificado de autoridad emisora de certificados (normalmente llamado paquete de autoridad de certificado).
   * Debe tener una clave privada coincidente y un certificado para poder utilizar un certificado.
11. Vuelva a la *<span style="text-decoration: underline">Configuración de alojamiento web</span>* de la configuración de Dominio.
12. Seleccione el certificado correspondiente y pulse **Aceptar**.

El nuevo certificado empieza a utilizarse para el dominio. Si ha actualizado el certificado, es posible que deba cerrar completamente el navegador antes de utilizar el nuevo certificado.
