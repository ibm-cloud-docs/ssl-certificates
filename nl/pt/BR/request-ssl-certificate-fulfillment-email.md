---
copyright: years: 1994, 2017 lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Solicitando um e-mail de preenchimento de certificado SSL

## Visão geral

Depois de pedir um novo certificado SSL por meio do {{site.data.keyword.BluSoftlayer_full}}, a autoridade de certificação envia um e-mail de preenchimento para o administrador de domínio fornecido durante o processo de pedido. Esse e-mail contém todos os detalhes associados ao certificado SSL. A qualquer momento, o e-mail de preenchimento pode ser solicitado novamente na tela de Pedidos SSL no {{site.data.keyword.slportal_full}}. Siga as etapas abaixo para solicitar o e-mail de preenchimento SSL da autoridade de certificação.

## Solicitando um e-mail de preenchimento

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Pedidos**.
3. Clique no link **Enviar** na coluna **E-mail** para o certificado SSL desejado.<br/>**Observação:** uma janela pop-up aparece para confirmar a solicitação. Essa janela contém o endereço de e-mail para o Administrador de Domínio que foi fornecido quando o certificado SSL foi solicitado.
4. Clique no botão **Reenviar e-mail** para confirmar a seleção e solicitar um e-mail de preenchimento adicional da autoridade de certificação.  Ou, clique em **Cancelar** para cancelar a ação.

## O que acontece em seguida

Depois de solicitar um e-mail de preenchimento adicional, a solicitação será encaminhada para a autoridade de certificação aplicável para conclusão. Como os detalhes do certificado SSL são confidenciais, o {{site.data.keyword.BluSoftlayer_notm}} não armazena os dados do certificado SSL em nosso sistema. Depois de receber os detalhes do certificado SSL por e-mail, eles podem ser manualmente [importados](import-ssl-certificate.html) para o {{site.data.keyword.slportal}}, se necessário.
