---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Excluindo certificados SSL
{: #deleting-ssl-certificates}

Depois que os detalhes de um certificado SSL são importados para o console do {{site.data.keyword.cloud}}, ele pode ser excluído a qualquer momento para remover todos os dados que seriam salvos no console do {{site.data.keyword.cloud_notm}}.

Para excluir um certificado SSL, conclua as etapas a seguir.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. No menu **Ações**, selecione **Excluir** para o certificado SSL desejado.
4. Clique em **Sim** para excluir o certificado SSL.

## Etapas seguintes

Depois de excluir um certificado SSL, nenhum serviço vinculado a ele usará mais suas informações. O certificado não aparece mais na tela Certificados SSL no console do {{site.data.keyword.cloud_notm}}.

Atualize todos os serviços que anteriormente usavam o certificado excluído para que sejam associados a um certificado SSL válido associado à conta.

A qualquer momento, o certificado SSL pode ser incluído de volta no console do {{site.data.keyword.cloud_notm}} usando o processo de [importação](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates).
{:note}
