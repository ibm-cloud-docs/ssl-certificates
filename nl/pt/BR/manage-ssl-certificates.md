---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gerenciando certificados SSL
{: #managing-ssl-certificates}

É possível gerenciar seus certificados SSL no console do {{site.data.keyword.cloud}}. Além de servir como um repositório para o gerenciamento dos certificados, isso também é necessário ao usar serviços que podem usar ou requerer certificados.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Certificados > Gerenciar certificados**.


Você será apresentado a uma lista atual de seus certificados com informações sobre seus status.

É possível procurar e fazer download de partes de um certificado ou de uma versão formatada por PEM ou revisar a expiração
de seus certificados. Também é possível visualizar quantos serviços cada certificado está usando atualmente. Isso permite saber se a
ação deve ser tomada quando um certificado está se aproximando da expiração.

## Incluindo um certificado

Quando você estiver pronto para incluir um certificado, selecione **Incluir certificado** no menu de subnavegação ou dentro do título Lista de certificados. Você só precisa fornecer o certificado e sua chave privada. No entanto, não fornecer um certificado
intermediário quando o seu emissor fornece um pode resultar em uma cadeia de certificados quebrada e uma validação incorreta para
usuários ou serviços associados.

As chaves privadas que requerem uma passphrase não podem ser armazenadas.
{:note}

Depois de incluído, os campos a seguir são derivados dos seus certificados diretamente:

* Nome comum
* Organization name
* Prazo de validade

## Editando um certificado

Ativar o triângulo à esquerda de um certificado revelará as partes do certificado em sua totalidade. Isso também permite que as partes do certificado sejam editadas. Uma nota pode ser incluída e, quando necessário, o certificado pode ser removido. Também listada há uma lista de serviços que estão atualmente usando o certificado.

Somente certificados que não estão associados a serviços podem ter suas partes de chave privada, de certificado ou de certificado intermediário atualizadas. O certificado também não pode ser removido. É possível modificar a nota em qualquer momento.

## Removendo um certificado

Para remover um certificado, siga as etapas para editá-lo e selecione "Confirmar remoção de certificado" e salve.

## Utilizando a API

Para obter um exemplo de edição de certificados usando a API, consulte
[Gerenciamento de SSL ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://sldn.softlayer.com/article/ssl-management){: new_window}.
