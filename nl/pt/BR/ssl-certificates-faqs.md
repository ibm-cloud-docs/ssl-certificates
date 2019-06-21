---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

# Perguntas frequentes: certificados SSL
{: #faqs-ssl-certificates}

## Por que o certificado SSL que eu solicitei não aparece automaticamente na tela de certificados SSL?
{:faq}

Certificados SSL são emitidos por uma autoridade de certificado de empresa terceirizada, que envia todos os detalhes do
certificado diretamente para você em um e-mail confidencial. Depois de receber esse e-mail, você tem a opção de [importar o certificado SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) para o console do {{site.data.keyword.cloud}}, caso você escolha usar o certificado com produtos e serviços do {{site.data.keyword.cloud_notm}}. Como {{site.data.keyword.cloud_notm}} nunca recebe os detalhes para o certificado SSL, os dados não podem ser importados automaticamente.

## O que é um certificado SSL?
{:faq}

Certificados SSL são ativados por websites como uma medida de segurança para proteger o usuário. Geralmente, eles são usados quando é necessário que você transmita informações confidenciais para um website, como nome, endereço, números de cartão de crédito e outros dados pessoais, ou quando está gerenciando dados que requerem autenticação (como no console do {{site.data.keyword.cloud_notm}}). Certificados SSL são solicitados pela empresa que administra o website, mas são emitidos por uma empresa terceirizada confiável que assegura a validade do website. Websites seguros são precedidos por HTTPS na URL, em vez de HTTP padrão.

## Como posso solicitar um SSL SHA2?
{:faq}

Se você já solicitou um SSL e ele estiver mostrando erros de que o certificado SSL está usando SHA-1 em vez de SHA-2, será
necessário solicitar que o SSL seja emitido novamente. É possível fazer isso enviando um chamado.

Se você ainda não tiver pedido um SSL do {{site.data.keyword.cloud_notm}} e precisar solicitar um com SHA-2, envie um
chamado para solicitar manualmente um SSL para o domínio em questão. O console do {{site.data.keyword.cloud_notm}} ainda cria automaticamente os certificados SSL usando SHA-1, portanto, se você fizer isso, será necessário que ele seja emitido novamente.
