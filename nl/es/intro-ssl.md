---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: SSL certificate, SSL technology, public key

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introducción a la tecnología SSL
{: #introduction-to-ssl-technology}

La capa de sockets seguros (SSL) es una tecnología que cifra el tráfico entre la aplicación del cliente y la del servidor. El cifrado se logra mediante el uso de un sistema de clave pública/clave privada que utiliza un certificado SSL. El certificado SSL contiene la clave pública del servidor, fechas en las cuales es válido el certificado, un nombre de host para el cual el certificado es válido y una firma de la autoridad de certificación que lo haya emitido.
{:shortdesc}

## Terminología SSL

Las certificaciones SSL tienen una terminología única. Al trabajar con certificados SSL, puede encontrarse los términos siguientes.

### Tamaño en bits
Las claves de cifrado se miden por su tamaño en bits. Por ejemplo 512 bits, 1024 bits, 2048 bits. Generalmente, una clave larga será más segura pero más lenta de utilizar. En este momento, el tamaño mínimo de las claves que se utilizan en certificados SSL es de 1024 bits, aunque los certificados de validación ampliada requieren 2048 bits.

### Cadena de certificados
Normalmente los certificados SSL no se utilizan solos. En la mayoría de implementaciones se trabaja con una cadena de certificados. Por ejemplo:

    Root > intermediate1 > server cert.

    \> Intermediate2 > server2 cert

En este ejemplo, el certificado de servidor lo firma el certificado intermedio, que, a su turno, lo firma el certificado raíz. Encadenar de este modo, puede hacer que la SSL sea más segura, ya que de esta forma el certificado raíz no se utiliza (ni se expone a riesgos) tan a menudo. Si `intermediate1` estuviera en peligro, el `certificado del servidor` podría estar en peligro, pero `server2 cert` estaría bien porque forman parte de distintas cadenas.

### Solicitud de firma de certificado
Una solicitud de firma de certificado (CSR) es un documento que genera en el servidor que contiene información que la autoridad de certificación utiliza para crear el certificado.

### Nombre común
El nombre común (CN) es el nombre de host para el cual el certificado es válido (por ejemplo, www.domain.com).  

 www.domain.com, smtp.domain.com y mail.domain.com son tres nombres de host diferentes y el mismo certificado SSL no es válido para los tres (excepto si utiliza un certificado comodín, pero actualmente {{site.data.keyword.cloud}} no los ofrece).
 {:note}

### Clave privada/pública
SSL utiliza una técnica denominada criptografía de clave pública. En esta forma de criptografía, tiene dos claves: la pública y la privada. La clave pública se distribuye por todas partes. Nadie ve su clave privada. Los usuarios que desean comunicarse de forma segura con usted cifran sus comunicaciones con su clave pública. La criptografía de clave pública se basa en la aserción de que los bits cifrados con una determinada clave pública solo pueden ser descifrados con la correspondiente clave privada y viceversa.

### Certificado raíz
Los certificados raíz SSL son certificados que se han autofirmado y que han presentado sus respectivas Autoridades de certificación como parte superior de su cadena. Encontrará certificados raíz de Autoridades de certificación ya instalados en el almacén de certificados de su navegador web. Esto permite que su navegador confíe en dichos certificados y forma los inicios de las cadenas de confianza que llevan al certificado que instala en su servidor.

### Firma
La autoridad emisora de certificados coloca una firma digital en los certificados SSL. Esta firma, una vez trazada hasta un certificado raíz de confianza, confirma la autenticidad del certificado.

## SSL en la infraestructura de IBM Cloud

{{site.data.keyword.cloud}} revende tres tipos de certificados de SSL: Validación de dominio, Validación de organización, Validación ampliada.

Los certificados de Validación de dominio (DV) son baratos y están disponibles rápidamente. La validación que realiza la autoridad de certificación se limita a enviar un correo electrónico a una dirección de correo electrónico concreta en el dominio en cuestión y a obtener una respuesta positiva. Los certificados de Validación de organización (OV) y la Validación ampliada (EV) tardan dos días (a veces más), cuestan más y suponen más comprobaciones por parte de la autoridad de certificación. Los certificados de EV se codifican de manera que los navegadores los reconocen como EV y muestran una barra verde como parte de la barra de direcciones.

Los certificados SSL, igual que otros servicios de {{site.data.keyword.cloud_notm}}, se pueden gestionar a través de la consola de {{site.data.keyword.cloud_notm}}. Vaya al menú **Seguridad** y seleccione la opción **SSL** para solicitar y gestionar certificados.  

Los certificados SSL solicitados mediante {{site.data.keyword.cloud_notm}} no tienen que utilizarse en un servidor {{site.data.keyword.cloud_notm}}. Además, los certificados solicitados en otro lugar se pueden utilizar en los servidores que se alojan aquí.
{:note}

Los certificados SSL mejoran la seguridad de las transacciones que se realizan y proporcionan a los usuarios una sensación de seguridad. Además de los certificados SSL, la seguridad Daemon, la seguridad física, las prácticas de codificación y la gestión de certificados se combinan para formar el perfil de seguridad general de la solución.

