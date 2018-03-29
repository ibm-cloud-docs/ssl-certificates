---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Excluindo certificados SSL

Após a importação dos detalhes de um certificado SSL para o {{site.data.keyword.slportal_full}}, ele
poderá ser excluído a qualquer momento para evitar que todos os dados sejam salvos no {{site.data.keyword.slportal}}.

Para excluir um certificado SSL, conclua as etapas a seguir.

1. Acesse o [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. No menu **Ações**, selecione **Excluir** para o certificado SSL desejado.

  **Observação:** uma janela é exibida para confirmar a exclusão.
4. Clique em **Sim** para excluir o certificado SSL ou clique em **Não** para cancelar a ação.

## Próximas Etapas

Depois de excluir um certificado SSL, nenhum serviço vinculado a ele usará mais suas informações. O certificado não aparece mais na tela de certificados SSL no {{site.data.keyword.slportal}}.

Recomenda-se que você atualize todos os serviços que anteriormente usaram o certificado excluído para serem associados a um certificado SSL válido associado à conta.

**Nota:** a qualquer momento, o certificado SSL pode ser incluído de volta no
{{site.data.keyword.slportal}} usando o processo de [importação](import-ssl-certificate.html).
