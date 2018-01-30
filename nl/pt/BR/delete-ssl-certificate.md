---
copyright: years: 1994, 2017 lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Excluindo certificados SSL

## Visão geral

Após os detalhes de um certificado SSL serem importados para o {{site.data.keyword.slportal_full}}, ele pode ser excluído a qualquer momento para remover todos os dados de serem salvos no {{site.data.keyword.slportal}}.

Para excluir um certificado SSL, conclua as etapas a seguir.

## Excluindo um certificado SSL

1. Acesse o [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. No menu **Ações**, selecione **Excluir** para o certificado SSL desejado.

  **Observação:** uma janela é exibida para confirmar a exclusão.
4. Clique em **Sim** para excluir o certificado SSL ou clique em **Não** para cancelar a ação.

## Próximas Etapas

Depois de excluir um certificado SSL, todos os serviços vinculados ao certificado não usarão mais suas informações. O certificado não aparece mais na tela de certificados SSL no {{site.data.keyword.slportal}}.

Recomenda-se que você atualize todos os serviços que anteriormente usaram o certificado excluído para serem associados a um certificado SSL válido associado à conta.

**Observação:** em qualquer momento, o certificado SSL pode ser incluído de volta para o {{site.data.keyword.slportal}} usando o processo de [importação](import-ssl-certificate.html).
