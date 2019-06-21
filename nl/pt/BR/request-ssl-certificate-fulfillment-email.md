---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Solicitando um e-mail de preenchimento de certificado SSL
{: #requesting-an-ssl-certificate-fulfillment-email}

Depois de pedir um novo certificado SSL por meio do {{site.data.keyword.cloud}}, a autoridade de certificação envia um e-mail de preenchimento para o administrador de domínio fornecido durante o processo de pedido. Esse e-mail contém todos os detalhes que estão associados com o certificado SSL. A qualquer momento, o e-mail de cumprimento pode ser solicitado novamente por meio da tela Pedidos de SSL no console do {{site.data.keyword.cloud_notm}}.
{:shortdesc}

## Solicitando um e-mail de preenchimento
Conclua as etapas a seguir para
solicitar o e-mail de cumprimento SSL da autoridade de certificação.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Pedidos**.
3. Clique no link **Enviar** na coluna **E-mail** para o certificado SSL que você
deseja.

  Uma janela pop-up aparece para confirmar a solicitação. Essa janela contém o endereço de e-mail para o administrador de domínio que foi fornecido quando o certificado SSL foi solicitado.
  {:note}

4. Clique em **Reenviar e-mail** para confirmar a seleção e solicitar um e-mail de cumprimento adicional
da autoridade de certificação.

## Etapas seguintes

Depois de solicitar um e-mail de preenchimento adicional, a solicitação será encaminhada para a autoridade de certificação aplicável para conclusão. Como os detalhes do certificado SSL são confidenciais, o {{site.data.keyword.cloud_notm}} não armazena os dados do
certificado SSL em seu sistema. Depois de receber os detalhes do certificado SSL por e-mail, eles podem ser [importados](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) manualmente para o console do {{site.data.keyword.cloud_notm}}, se necessário.
