---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renovando certificados SSL
{: #renewing-ssl-certificates}

Após o pedido de um certificado SSL por meio do {{site.data.keyword.cloud}}, ele pode ser
renovado a qualquer momento. Durante o processo de renovação, o {{site.data.keyword.cloud_notm}} age como o facilitador entre a autoridade de certificação e você, e não vê nem controla nenhuma parte do processo de renovação que envolve os detalhes do certificado SSL. Os certificados SSL são renovados sob os mesmos termos em que foram pedidos, portanto, nenhuma mudança nos detalhes de renovação (tipo de certificado e autoridade, mês de validade, plataforma do servidor e assim por diante) pode ser feita. Os certificados podem ser
renovados antes ou depois de expirarem; no entanto, para manter a validade do certificado SSL, renove o certificado antes da
data de expiração.
{:shortdesc}

## Renovando um certificado SSL
Conclua as etapas a seguir para renovar um certificado SSL.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Pedidos**.
3. Clique em **Renovar** na coluna **Renovar** para o certificado SSL desejado.
4. Determine se todos os detalhes da renovação e da CSR estão corretos antes de renovar o certificado SSL. Consulte a tabela a seguir para obter informações adicionais.  

| Detalhes                         | Ação  |
| ------------------------------- | ------- |
| Corrigir detalhes da renovação e da CSR | Selecione **Renovar** para renovar o certificado SSL. |
| Detalhes da renovação incorretos       | Selecione **Comprar um novo certificado SSL** para pedir um novo certificado. Como os detalhes de renovação, incluindo o tipo de certificado, a autoridade e o e-mail de aprovação não podem ser mudados, a única maneira de atualizar os detalhes para o certificado SSL de um website é pedir um novo certificado. |
| Detalhes da CSR incorretos           | Selecione **Mudar CSR**, insira os novos detalhes da CSR na caixa de texto **CSR** e selecione **Restaurar CSR**. |
{: caption="Tabela 1. Detalhes de renovação e de CSR" caption-side="top"}

## Etapas seguintes

Depois de solicitar a renovação de um certificado SSL, o {{site.data.keyword.cloud_notm}} encaminha
a solicitação para a autoridade de certificação para concluir a verificação de website necessária para a renovação. Após a renovação do certificado, a nova data de expiração aparecerá no campo **Expira**.
