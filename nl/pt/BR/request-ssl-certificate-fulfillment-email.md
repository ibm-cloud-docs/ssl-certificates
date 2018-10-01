---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Solicitando um e-mail de preenchimento de certificado SSL

Depois de pedir um novo certificado SSL por meio do {{site.data.keyword.BluSoftlayer_full}}, a autoridade de certificação envia um e-mail de preenchimento para o administrador de domínio fornecido durante o processo de pedido. Esse e-mail contém todos os detalhes que estão associados com o certificado SSL. A qualquer momento, o e-mail de cumprimento pode
ser solicitado novamente na tela Pedidos SSL no {{site.data.keyword.slportal_full}}. Conclua as etapas a seguir para
solicitar o e-mail de cumprimento SSL da autoridade de certificação.

## Solicitando um e-mail de preenchimento

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Pedidos**.
3. Clique no link **Enviar** na coluna **E-mail** para o certificado SSL que você
deseja.<br/>**Observação:** uma janela pop-up aparece para confirmar a solicitação. Essa janela contém o endereço de e-mail para o Administrador de Domínio que foi fornecido quando o certificado SSL foi solicitado.
4. Clique em **Reenviar e-mail** para confirmar a seleção e solicitar um e-mail de cumprimento adicional
da autoridade de certificação.  Ou, clique em **Cancelar** para cancelar a ação.

## Próximas Etapas

Depois de solicitar um e-mail de preenchimento adicional, a solicitação será encaminhada para a autoridade de certificação aplicável para conclusão. Como os detalhes do certificado SSL são confidenciais, o {{site.data.keyword.BluSoftlayer_notm}} não armazena os dados do
certificado SSL em seu sistema. Depois de receber os detalhes do certificado SSL por e-mail, eles podem ser manualmente
[importados](import-ssl-certificate.html) para o {{site.data.keyword.slportal}}, se necessário.
