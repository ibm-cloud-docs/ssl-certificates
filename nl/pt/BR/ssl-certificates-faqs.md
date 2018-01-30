---
copyright: years: 1994, 2017 lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

<a name="top"></a>
# Perguntas frequentes: certificados SSL

## Por que o certificado SSL que eu solicitei não aparece automaticamente na tela de certificados SSL?

Os certificados SSL são emitidos por uma Autoridade de certificação de terceiros, que envia todos os detalhes do certificado diretamente para você em um e-mail confidencial. Depois de receber o e-mail, você tem a opção de[importar o certificado SSL](import-ssl-certificate.html) para o {{site.data.keyword.slportal_full}}. É necessário escolher usar o certificado com produtos e serviços {{site.data.keyword.BluSoftlayer_full}}. Como nunca recebemos os detalhes do certificado SSL, não podemos importar esses dados automaticamente.

## O que é um certificado SSL?

Os certificados SSL são ativados por websites como uma medida de segurança para proteger o usuário final. Eles geralmente são utilizados quando você é obrigado a transmitir informações confidenciais a um website, como nome, endereço, números de cartão de crédito e outros dados pessoais ou quando você está gerenciando dados que exigem autenticação (como dentro de nosso {{site.data.keyword.slportal}}). Certificados SSL são solicitados pela empresa que administra o website, mas são emitidos por uma empresa terceirizada confiável que assegura a validade do website. Websites seguros serão precedidos por HTTPS na URL, em vez de HTTP padrão.

## Como posso solicitar um SSL SHA2?

Se você já solicitou um SSL e ele estiver mostrando erros de que o certificado SSL está usando o SHA-1 em vez do SHA-2, será necessário solicitar que voltem a emitir o SSL. É possível fazer isso enviando um chamado.

Se você ainda não tiver solicitado um SSL e precisar de um com SHA-2, envie um chamado para fazer a solicitação manual de um SSL para o domínio em questão. Nosso portal ainda cria automaticamente certificados SSL usando SHA-1, então, se você fizer isso, será necessário que ele seja emitido novamente.
