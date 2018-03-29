---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Planificación para SSL

Iniciarse en SSL requiere algo de planificación. Lleve a cabo los siguientes requisitos previos.

1. Decida de dónde obtener el certificado
2. Obtenga información sobre los tipos de certificados, la longitud de las claves y la duración
3. Seleccione un nombre común
4. Obtenga información sobre la regla de sockets
5. Genere el CSR

## Decida de dónde obtener el certificado

Los certificados SSL pueden obtenerse internamente en su organización o desde una Autoridad de certificación, como Verisign, RapidSSL o Thawte, entre otros.  

Para un grupo pequeño en una arquitectura controlada, como empleados que utilizan un sitio de Intranet, puede adquirir un certificado autofirmado que cada empleado instale en su navegador. También puede configurar su propia autoridad de certificación local para generar certificados para utilizar en su organización.

Para un grupo más amplio y diverso, el uso de un certificado SSL de una fuente estándar permite el acceso sin una configuración especializada. Los navegadores web modernos se configuran para que confíen en los certificados SSL emitidos por Autoridades de certificación.

## Obtenga información sobre los tipos de certificados, la longitud de las claves y la duración

Una vez que haya decidido de dónde obtener el certificado, revise las opciones siguientes para los tipos de certificados y su correspondiente disponibilidad, longitud de clave y duración.

|              Tipos de certificado       |  Disponibilidad                   |  Longitud de la clave      |  Duración                  |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Validación de dominio (DV)               | Disponible rápidamente            | 1024 bits o 2048 bits      | 1 o 2 años                 |
|Validación de organización (OV)          | 2-3 días o hasta una semana       | 1024 bits o 2048 bits      | 1 o 2 años                 |
|Validación ampliada (EV)                 | 2-3 días o hasta una semana       | Solo 2048 bits             | 1 o 2 años                 |
{: caption="Tabla 1. Tipos de certificado" caption-side="top"}   


## Seleccione un nombre común

El nombre común utilizado en el certificado es el nombre de host para el sitio web. El nombre de host y el nombre común del certificado deben coincidir; de lo contrario, los navegadores emitirán una advertencia. Si, por ejemplo, su sitio es web1.mydomain.com, utilícelo como nombre común. Si también utiliza images.mydomain.com, necesita o bien un certificado comodín (que no está disponible en {{site.data.keyword.cloud}}) o bien debe configurar varios certificados. Si elige un nombre incorrecto, hay pasos que pueden seguirse para arreglar un pedido de certificado o para revocar y volver a emitir el nombre común correcto.  

## Obtenga información sobre la regla de sockets

Hay un límite de un certificado por socket. Un socket es una dirección IP y una combinación de puertos, como 1.2.3.4:443. 1.2.3.4:444 sería un socket distinto. Esto no es importante para aplicaciones como SMTP/POP3 o FTP. Sin embargo, es importante para HTTP por su implicación en el alojamiento virtual.

El alojamiento virtual es el método mediante el cual puede alojar 20, 30, 100 sitios web en una dirección IP. Funciona porque los navegadores modernos pasan un campo llamado lector de host como parte de su solicitud. Este campo tiene el aspecto “Host: web1.mydomain.com” e informa al servidor web sobre el sitio al cual intenta acceder. En el caso de HTTPS (HTTP sobre SSL), el servidor web debe seleccionar el certificado SSL para enviar al cliente antes de ver la cabecera de host, motivo por el cual un socket solo puede tener un certificado.

Puede asignar cada sitio web habilitado para SSL a su propio socket. Puede hacerlo cambiando la dirección IP o el puerto. Recuerde que, si cambia el puerto de 443/tcp, los usuarios tienen que incluir el número de puerto en su URL como https://web1.mydomain.com:444.

## Genere el CSR

Puede generar la Solicitud de firma de certificado mediante el software del servidor web. Para sistemas UNIX, utilice el paquete OpenSSL. Para Windows, hay un asistente al cual se accede desde el separador Seguridad del directorio de las propiedades del sitio web en el Gestor IIS. Si utiliza un panel de control, consulte la información concreta sobre este panel de control.

Durante la creación del CSR, creará una clave privada. No pierda, borre ni comparta la clave privada. Debe mantenerse privada en el servidor web. Algunas utilidades de la generación CSR también le ofrecen la posibilidad de crear una contraseña para la clave privada. No la crea a menos que planee iniciar sesión en el servidor cada vez que el software del servidor web se reinicie. No aplique tampoco una frase de desafío al CSR.

