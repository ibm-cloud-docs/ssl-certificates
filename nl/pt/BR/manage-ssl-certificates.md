---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Gerenciando certificados SSL

O {{site.data.keyword.BluSoftlayer_full}} agora fornece um meio de armazenar certificados em seu portal. Além de servir como um repositório para o gerenciamento dos certificados, isso também é necessário ao usar serviços que podem usar ou requerer certificados.

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados > Gerenciar certificados**.

Você será apresentado a uma lista atual de seus certificados com informações sobre seus status.

É possível procurar e fazer download de partes de um certificado ou de uma versão formatada por PEM ou revisar a expiração
de seus certificados. Também é possível visualizar quantos serviços cada certificado está usando atualmente. Isso permite saber se a
ação deve ser tomada quando um certificado está se aproximando da expiração.

## Incluindo um certificado

Quando estiver pronto para incluir um certificado, selecione "Incluir certificado" no menu de subnavegação ou no título da
Lista de certificados. Você só precisa fornecer o certificado e sua chave privada. No entanto, não fornecer um certificado
intermediário quando o seu emissor fornece um pode resultar em uma cadeia de certificados quebrada e uma validação incorreta para
usuários ou serviços associados.

Observação: as chaves privadas que requerem uma passphrase não podem ser armazenadas.

Depois de incluído, os campos a seguir são derivados dos seus certificados diretamente:

* Nome comum
* Nome da organização
* Período de validade

## Editando um certificado

Ativar o triângulo à esquerda de um certificado revelará as partes do certificado em sua totalidade. Isso também permite que as partes do certificado sejam editadas. 
Uma nota pode ser incluída e, quando necessário, o certificado pode ser removido. Também listada há uma lista de serviços que estão atualmente usando o certificado.

**Nota**: somente certificados que não estão associados a serviços podem ter as partes "chave
privada", "certificado" ou "certificado intermediário" atualizadas. O certificado também não pode ser removido.

É possível modificar a nota em qualquer momento.

## Removendo um certificado

Para remover um certificado, siga as etapas para editá-lo e selecione "Confirmar remoção de certificado" e salve.

### API

Para obter um exemplo de edição de certificados usando a API, consulte
[Gerenciamento de SSL ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](http://sldn.softlayer.com/article/ssl-management){: new_window}. 
