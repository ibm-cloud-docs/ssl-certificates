---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates, common name, SSL certificates

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Planning for SSL
{: #planning-for-ssl}

Getting started with SSL requires a bit of planning. Complete the following prerequisites.

1. Decide where to get the certificate
2. Learn about the types of certificates, key length, and duration
3. Choose a common name
4. Learn about the socket rule
5. Generate the CSR

## Decide where to get the certificate

SSL certificates can be obtained internally in your organization or from a certificate authority, such as Verisign, RapidSSL, Thawte, and others.  

For a small group in a controlled architecture, such as employees who use an intranet site, you can acquire a Self-Signed certificate that each employee installs in their browser. You can also set up a local certificate authority of your own to generate certificates for use in your organization.

For a larger, more diverse group, using an SSL certificate from a standard source allows access without specialized configuration. Modern web browsers are configured to trust SSL certificates that are issued by certificate authorities.

## Learn about the types of certificates, key length, and duration

After you decide where to get your certificate, review the following options for certificate types and their corresponding availability, key length, and duration.

|              Certificate Types          |  Availability                     |  Key Length                |  Duration                  |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Domain Validation (DV)                   | Quickly available                 | 1024 bit or 2048 bit       | 1 or 2 year(s)             |
|Organization Validation (OV)             | 2-3 days or up to a week          | 1024 bit or 2048 bit       | 1 or 2 year(s)             |
|Extended Validation (EV)                 | 2-3 days or up to a week          | 2048 bit only              | 1 or 2 year(s)             |
{: caption="Table 1. Certificate types" caption-side="top"}   


## Choose a common name

The common name that is used in the certificate is the host name for the website. The host name and the common name of the certificate must match, or browsers issue a warning. If your site is web1.mydomain.com, then make that your common name. If you also use images.mydomain.com, you need either a wildcard certificate (which is not available from {{site.data.keyword.cloud}}) or you need to set up multiple certificates. If you choose the wrong common name, there are steps that can be taken to fix a certificate order or to revoke and reissue with the correct common name.  

## Learn about the socket rule

SSL certificates are limited to one certificate per socket. A socket is an IP address and port combination, such as 1.2.3.4:443 (1.2.3.4:444 would be a different socket). For applications like SMTP/POP3 or FTP, the socket rule does not matter. However, it matters for HTTP because of its involvement with virtual hosting.

Virtual hosting is the method by which you can host 20, 30, 100 websites on one IP address. Virtual hosting works because modern browsers pass a field that is called the host reader as part of their request. This field looks like “Host: web1.mydomain.com” and tells the web server which site you are trying to access. In the case of HTTPS (HTTP over SSL), the web server must select the SSL certificate to send to the client before seeing the host header, which is why a socket can have only one certificate.

You can assign each SSL-enabled website to its own socket by varying the IP address or varying the port. Keep in mind if you change the port from 443/tcp, users must include the port number in their URL like `https://web1.mydomain.com:444`.

## Generate the CSR

You can generate the certificate signing request (CSR) by using software on the web server. For UNIX systems, use the OpenSSL package. For Windows, there is a wizard that is accessed from the Directory Security tab of the website properties in IIS Manager. If you are using a control panel, refer to specific information for that control panel.

While generating the CSR, you create a private key. Do not lose, delete, or share the private key. It is to be kept private on the web server. Some CSR generation utilities also give you the ability to create a passphrase for the private key. Do not do this unless you plan to log on to the server any time the web server software is restarted. In addition, do not apply a challenge phrase to the CSR.

