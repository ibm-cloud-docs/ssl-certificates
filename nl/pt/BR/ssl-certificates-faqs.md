---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Perguntas frequentes: certificados SSL

## Por que o certificado SSL que eu solicitei não aparece automaticamente na tela de certificados SSL?

Certificados SSL são emitidos por uma autoridade de certificado de empresa terceirizada, que envia todos os detalhes do
certificado diretamente para você em um e-mail confidencial. Depois de receber o e-mail, você tem a opção de[importar o certificado SSL](import-ssl-certificate.html) para o {{site.data.keyword.slportal_full}}. É necessário escolher usar o certificado com produtos e serviços {{site.data.keyword.BluSoftlayer_full}}. Como {{site.data.keyword.cloud_notm}} nunca recebe os detalhes para o certificado SSL, os dados não podem ser importados automaticamente.

## O que é um certificado SSL?

Certificados SSL são ativados por websites como uma medida de segurança para proteger o usuário. Geralmente eles são
usados quando você é obrigado a transmitir informações confidenciais a um website, como nome, endereço, números de cartão de
crédito e outros dados pessoais ou está gerenciando dados que requerem autenticação (como no {{site.data.keyword.slportal}}). Certificados SSL são solicitados pela empresa que administra o website, mas são emitidos por uma empresa terceirizada confiável que assegura a validade do website. Websites seguros são precedidos por HTTPS na URL, em vez de HTTP padrão.

## Como posso solicitar um SSL SHA2?

Se você já solicitou um SSL e ele estiver mostrando erros de que o certificado SSL está usando SHA-1 em vez de SHA-2, será
necessário solicitar que o SSL seja emitido novamente. É possível fazer isso enviando um chamado.

Se você ainda não tiver pedido um SSL do {{site.data.keyword.cloud_notm}} e precisar solicitar um com SHA-2, envie um
chamado para solicitar manualmente um SSL para o domínio em questão. O {{site.data.keyword.slportal}} ainda cria
automaticamente certificados SSL usando SHA-1, então, se você fizer isso, será necessário emiti-lo novamente.
