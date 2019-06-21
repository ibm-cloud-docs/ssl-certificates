---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate details, preferred Download Option, SSL certificate download details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Fazendo download dos detalhes do certificado SSL
{: #downloading-ssl-certificate-details}

Depois que um certificado SSL é incluído no console do {{site.data.keyword.cloud}}, seus detalhes podem ser transferidos por download a qualquer momento. Os downloads podem incluir o certificado, a chave ou o PEM, que inclui todos os detalhes disponíveis associados ao certificado SSL. Os detalhes do certificado SSL são transferidos por download com segurança,
assim, não há nenhum risco associado à recuperação dos detalhes por meio desse método.
{:shortdesc}

Para fazer download dos detalhes para o certificado SSL, conclua as etapas a seguir.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. No menu **Ações**, selecione a **Opção de download** preferida para o
certificado. Consulte a tabela a seguir para obter mais informações:

| Opção de download      | Informações de Download |
| -------------------- | -------------------- |
| Certificado de download | Faz download somente da parte do certificado e não inclui os detalhes da chave privada, do certificado intermediário, da solicitação de assinatura de certificado ou das notas. |
| Fazer Download de Chave         | Faz download apenas da chave privada e não inclui os detalhes do certificado, do certificado intermediário, da solicitação de assinatura de certificado ou das notas. |
| Download do PEM         | Faz download de todos os detalhes que estão associados ao certificado SSL, incluindo os detalhes do certificado, da chave privada, do certificado intermediário, da solicitação de assinatura de certificado e das notas. |
{: caption="Tabela 1. Opções de download" caption-side="top"}

## Etapas seguintes

Após solicitar os detalhes do certificado SSL para download, eles são automaticamente transferidos por download no navegador da web. Selecione o download para abrir o arquivo. O arquivo também pode ser salvo em sua estação de trabalho para referência futura. No
entanto, os dados para qualquer certificado SSL presente na tela de certificados SSL podem ser transferidos por download
automaticamente a qualquer momento repetindo as etapas anteriores.

