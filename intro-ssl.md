---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-30"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introduction to SSL technology

Secure Sockets Layer (SSL) is a technology that encrypts traffic between the client application and the server application. This encryption is accomplished by making use of a public key/private key system using an SSL certificate.

The SSL certificate contains the server’s public key, dates for which the certificate is valid, a hostname for which the certificate is valid, and a signature from the certification authority that issued it.

## SSL terminology

SSL certificates have unique terminology. You might encounter the following terms while working with SSL certificates.

**Bit size:** Encryption keys are measured by their size in bits. For example 512 bit, 1024 bit, 2048 bit. Generally, a longer key is going to be safer but slower to use. At this time, the minimum size for the keys used in SSL certificates is 1024 bit, though the Extended Validation certificates require 2048 bit.

**Certificate Chain:** SSL certificates are not generally used alone. In most implementations you will actually be dealing with a certificate chain. For example:

  Root > intermediate1 > server cert.

  \> Intermediate2 > server2 cert

In this example, your server certificate is signed by the intermediate certificate, which is in turn signed by the root certificate. Chaining in this fashion can make SSL more secure because it means that the root certificate is not used (and exposed to risk) so often. If intermediate1 was compromised then server cert could be in danger but server2 cert would be fine because they are part of different chains.

**Certificate Signing Request:** The CSR is a document you generate on the server which contains information that the certification authority uses to create your actual certificate.

**Common Name:** The Common Name (CN) is the hostname for which the certificate is valid (for example, www.domain.com).  

*Note:* www.domain.com, smtp.domain.com, and mail.domain.com are three completely different hostnames and the same SSL certificate is not valid for all three of them (unless you are using a wildcard certificate but at this time {{site.data.keyword.cloud}} does not offer those).

**Private/Public Key:** SSL makes use of a technique called public key cryptography. In this form of cryptography, you have two keys: the public and the private. The public key is distributed far and wide. No one sees your private key. People who wish to communicate securely with you encrypt their communication using your public key. Public key cryptography is based upon the assertion that bits encrypted with a given public key can only be decrypted using the corresponding private key and vice versa.

**Root certificate:** The SSL root certificates are certificates that have signed themselves and have been presented to the world by their respective Certification Authorities as the top of their chain. You will find root certificates for Certification Authorities already installed in the certificate store for your web browser. This allows your browser to trust those certificates and forms the beginnings of the chain of trust leading ultimately to the certificate you install on your server.

**Signature:** SSL certificates have a digital signature placed upon them by the certification authority. This signature, when traced back to a trusted root certificate, confirms the authenticity of the certificate.

## SSL at IBM Cloud infrastructure

{{site.data.keyword.BluSoftlayer_full}} resells three types of SSL certificates: Domain Validation, Organization Validation, and Extended Validation. 

Domain validation (DV) certificates are inexpensive and available quickly. The validation done by the Certification Authority is limited to sending an email to a specified email address at the domain in question and getting a positive reply back. Organization Validation (OV) and Extended Validation (EV) certificates take a couple of days (sometimes a week), cost more, and result in deeper checks by the Certification Authority. The EV certificates are coded in such a way that browsers recognize them as EV and will typically display a green bar as part of the address bar. 

SSL certificates, like other {{site.data.keyword.cloud_notm}} services, can be managed through the {{site.data.keyword.slportal}}.  Go to the **Security** menu and select the **SSL certificates** option at the bottom to order and manage certificates.  

**Note:** SSL certificates ordered through {{site.data.keyword.cloud_notm}} do not have to be used on a {{site.data.keyword.BluSoftlayer_notm}} server. In addition, certificates ordered elsewhere can be used on your servers hosted here.

**Conclusion**

SSL certificates enhance the security of the transactions taking place and give your users a sense of security. In addition to SSL certificates, Daemon security, physical security, coding practices, and certificate handling all combine to form the overall security profile of the solution.
