---
copyright:
  years: 2014, 2018
lastupdated: "2018-05-16"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Planejamento para SSL

A introdução ao SSL requer um pouco de planejamento. Conclua os pré-requisitos a seguir.

1. Decida onde obter o certificado
2. Saiba mais sobre os tipos de certificados, o comprimento da chave e a duração
3. Escolha um nome comum
4. Saiba mais sobre a regra do soquete
5. Gere o CSR

## Decida onde obter o certificado

Certificados SSL podem ser obtidos internamente em sua organização ou de uma autoridade de certificação, como Verisign, RapidSSL, Thawte e outros.  

Para um grupo pequeno em uma arquitetura controlada, como funcionários que usam um site de intranet, é possível adquirir um certificado autoassinado que cada funcionário instala em seu navegador. Também é possível configurar uma autoridade de certificação local da sua própria autoridade de certificação para gerar certificados para uso em sua organização.

Para um grupo maior e mais diversificado, usar um certificado SSL de uma fonte padrão permite acesso sem configuração especializada. Navegadores da web modernos são configurados para confiar em certificados SSL emitidos por autoridades de certificação.

## Saiba mais sobre os tipos de certificados, o comprimento da chave e a duração

Depois de decidir onde obter o seu certificado, reveja as seguintes opções para os tipos de certificados e sua disponibilidade correspondente, duração da chave e duração.

|              Tipos de Certificado          |  Disponibilidade                     |  Comprimento da chave                |  Duração                  |
| --------------------------------------- | --------------------------------- | -------------------------- | -------------------------- |
|Validação de domínio (DV)                   | Disponível rapidamente                 | 1024 bits ou 2048 bits       | 1 ou 2 anos             |
|validação de organização (OV)             | 2 a 3 dias ou até uma semana          | 1024 bits ou 2048 bits       | 1 ou 2 anos             |
|Validação estendida (EV)                 | 2 a 3 dias ou até uma semana          | Somente 2048 bits              | 1 ou 2 anos             |
{: caption="Tabela 1. Tipos de certificado" caption-side="top"}   


## Escolha um nome comum

O nome comum usado no certificado é o nome do host para o website. O nome do host e o nome comum do certificado devem corresponder ou os navegadores emitirão um aviso. Se o seu site for web1.mydomain.com, então certifique-se de que esse seja seu nome comum. Se você também usa images.mydomain.com, é necessário ter um certificado curinga (que não está disponível em {{site.data.keyword.cloud}}) ou configurar vários certificados. Se você escolher o nome comum errado, algumas etapas poderão ser executadas para corrigir uma ordem de certificado ou revogar e emitir novamente com o nome comum correto.  

## Saiba mais sobre a regra do soquete

Os certificados SSL são limitados a um certificado por soquete. Um soquete é uma combinação de endereço IP e porta, como 1.2.3.4:443 (1.2.3.4:444 seria um soquete diferente). Para aplicativos como SMTP/POP3 ou FTP, a regra de soquete não importa. No entanto, importa para HTTP devido a seu envolvimento com hospedagem virtual.

Hospedagem virtual é o método pelo qual você pode hospedar 20, 30, 100 websites em um endereço IP. Isso funciona porque os navegadores modernos passam um campo que é chamado de leitor de host como parte de sua solicitação. Esse campo se parece com “Host: web1.mydomain.com” e informa ao servidor da web qual site você está tentando acessar. No caso de HTTPS (HTTP sobre SSL), o servidor da web deve selecionar o certificado SSL para enviar ao cliente antes de ver o cabeçalho do host, e é por isso que um soquete pode ter apenas um certificado.

É possível atribuir cada website ativado para SSL a seu próprio soquete, variando o endereço IP ou variando a porta. Lembre-se de que, se você mudar a porta de 443/tcp, os usuários deverão incluir o número da porta na URL deles, como https://web1.mydomain.com:444.

## Gere o CSR

É possível gerar a Solicitação de Assinatura de Certificado usando software no servidor da web. Para sistemas UNIX, use o pacote OpenSSL. Para o Windows, há um assistente que é acessado na guia Segurança de diretório das propriedades do site em IIS Manager. Se você estiver usando um painel de controle, consulte as informações específicas sobre ele.

Ao gerar o CSR, você criará uma chave privada. Não perca, exclua ou compartilhe a chave privada. Ela deve ser mantida privada no servidor da web. Alguns utilitários de geração de CSR também fornecem a capacidade de criar uma passphrase para a chave privada. Não faça isso, a menos que você planeje efetuar logon no servidor sempre que o software do servidor web for reiniciado. Além disso, não aplique uma frase desafio para o CSR.

