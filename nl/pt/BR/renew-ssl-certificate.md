---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Renovando certificados SSL

Após o pedido de um certificado SSL por meio do {{site.data.keyword.BluSoftlayer_full}}, ele pode ser
renovado a qualquer momento. Durante o processo de renovação, o {{site.data.keyword.BluSoftlayer_notm}} age como facilitador entre o cliente (você) e a Autoridade de certificação e não vê ou controla qualquer parte do processo de renovação que envolve os detalhes do certificado SSL. 
Certificados SSL são renovados sob os mesmos termos em que foram pedidos, assim, nenhuma mudança nos detalhes de renovação (tipo
e autoridade de certificado, mês de validade, plataforma do servidor e assim por diante) pode ser feita. Os certificados podem ser
renovados antes ou depois de expirarem; no entanto, para manter a validade do certificado SSL, renove o certificado antes da
data de expiração. Conclua as etapas a seguir para renovar um certificado SSL.

## Renovando um certificado SSL

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Pedidos**.
3. Clique no link **Renovar** na coluna **Renovar** para o certificado SSL desejado.

   **Observação:** uma caixa pop-up aparecerá para concluir a solicitação.  
   * Determine se todos os detalhes de Renovação e de CSR estão corretos:<br /><br /><table border="1"><tr><th>Se...</th><th>Então...</th></tr><tr><td>Todos os detalhes da Renovação e CSR estão corretos</td><td>Continue com a próxima etapa.</td></tr><tr><td>Os detalhes de Renovação estão incorretos</td><td><ul><li>Clique no link <strong>Compre um novo certificado SSL</strong> para ser redirecionado para a tela de compra.<br /><blockquote><strong>Observação:</strong> como não é possível mudar os detalhes de Renovação, incluindo o Tipo de certificado, a Autoridade e o E-mail de aprovação, a única maneira de atualizar os detalhes de um certificado SSL de site é pedir um novo certificado.</blockquote></li><li>Conclua as telas na página Pedido com as informações desejadas para o certificado SSL. Nenhuma ação adicional será necessária ao usar esse procedimento.</li></ul></td></tr><tr><td>Detalhes do CSR são incorretos</td><td><ul><li>Clique no botão **Mudar CSR**.</li><li>Insira os **novos detalhes de CSR** na caixa de texto **CSR**.</li><li>Clique no botão **Restaurar CSR**.</li></ul></td></tr></table>
4. Clique no botão **Renovar** para renovar o certificado SSL ou clique em **Cancelar** para cancelar a ação.

## Próximas Etapas

Depois de solicitar a renovação de um certificado SSL, o {{site.data.keyword.BluSoftlayer_notm}} encaminha
a solicitação para a autoridade de certificação para concluir a verificação de website necessária para a renovação. Após a renovação
do certificado, a nova data de expiração aparece no campo Expira.
