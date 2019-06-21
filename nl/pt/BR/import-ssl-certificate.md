---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importando certificados SSL
{: #importing-ssl-certificates}

Depois que um certificado SSL é emitido para um website, ele pode ser importado para o console do {{site.data.keyword.cloud}}. Ao importar certificados SSL para o console do {{site.data.keyword.cloud_notm}}, os certificados podem ser aplicados a produtos e serviços que possam requerê-los, como a [transferência de SSL](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer) do Load Balancer. Por padrão, os certificados SSL que são emitidos pelo {{site.data.keyword.cloud_notm}} não são importados na lista,
pois se destinam a ser manipulados pelo destinatário somente. Portanto, qualquer certificado SSL usado com um produto ou um serviço {{site.data.keyword.cloud_notm}} deve ser importado manualmente por um usuário autorizado na conta.
{:shortdesc}

## Importando certificados SSL

Conclua as etapas a seguir para importar um certificado SSL.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. Clique em **Importar certificado SSL**.
4. Insira os **Detalhes do certificado SSL** nos campos aplicáveis e clique em **Importar**. Consulte a tabela a seguir para obter informações adicionais.

   Os detalhes que são inseridos na janela **Importar certificado SSL** devem ser
inseridos exatamente conforme fornecidos pela autoridade de certificação, incluindo espaçamento e quebras de linha. Se não, ocorre um erro.
   {:note}

| Detalhes do certificado SSL     | Descrição |
| --------------------------- | ----------- |
|Certificado                  | Detalhes do certificado SSL, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Chave privada                  | Detalhes da chave privada para o certificado, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|certificado intermediário     | Detalhes do certificado intermediário, fornecidos pela autoridade de certificação. Os certificados intermediários não são necessários. Porém, se as informações estiverem disponíveis para o certificado SSL, elas deverão ser inseridas.|
|Solicitação de assinatura de certificado  | Detalhes da solicitação de assinatura de certificado (CSR) fornecidos pela autoridade de certificação. Detalhes do CSR não são necessários, mas devem ser fornecidos se forem parte do certificado. **Observação:** não mude o CSR de forma alguma. Uma chave pública pode ser incluída com a CSR e não deve ser substituída pela chave privada.|
|Comunicados                        | Quaisquer notas referentes ao certificado SSL que podem ser úteis para outros usuários.|
{: caption="Tabela 1. Detalhes do certificado SSL" caption-side="top"}

## Etapas seguintes

Depois que o certificado SSL é importado para o console do {{site.data.keyword.cloud_notm}}, ele é armazenado na tela Certificados SSL até que seja [excluído manualmente](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates). Para todos os produtos ou
serviços que requerem detalhes do certificado SSL, o novo certificado SSL aparece na lista de certificados disponíveis para uso
ao interagir com o recurso SSL para o produto ou serviço procurado. O certificado pode ser
[atualizado](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates) e os detalhes sobre o certificado podem ser
[transferidos por download com segurança](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details) a qualquer momento.
