---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Importando certificados SSL

Após um certificado SSL ser emitido para um website, ele pode ser importado para o {{site.data.keyword.slportal_full}}. Ao importar certificados SSL para o {{site.data.keyword.slportal}}, os certificados podem ser aplicados a produtos e serviços que podem precisar deles, como a [Transferência SSL](/docs/infrastructure/local-load-balancer/configure-ssl-offloading-load-balancer.html){:new_window} do Load Balancer. 
Por padrão, os certificados SSL que são emitidos pelo {{site.data.keyword.BluSoftlayer_full}} não são importados na lista,
pois se destinam a ser manipulados pelo destinatário somente. Portanto, qualquer certificado SSL a ser usado com um produto ou serviço {{site.data.keyword.BluSoftlayer_notm}} deve ser importado manualmente por um usuário autorizado na conta. 
Conclua as etapas a seguir para importar um certificado SSL para o {{site.data.keyword.slportal}}.

## Importando certificados SSL

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. Clique no link **Importar certificado SSL** na parte superior da tela.
4. Insira os **Detalhes de certificado SSL** nos campos aplicáveis e clique em **Importar.**

   **Nota:** detalhes que são inseridos na janela **Importar certificado SSL** devem ser
inseridos exatamente como fornecidos pela autoridade de certificação, incluindo espaçamento e quebras de linha. Se não, ocorre um erro.

| Caixa de texto | Entrada |
| -------- | ----- |
|Certificado |Detalhes do certificado SSL, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Chave privada | Detalhes da chave privada para o certificado, fornecidos pela autoridade de certificação. Esse é geralmente um bloco alfanumérico de texto.|
|Certificado intermediário | Detalhes do certificado intermediário, fornecidos pela autoridade de certificação. Certificados intermediários não são necessários, no entanto, se a informação estiver disponível para o certificado SSL, ela deve ser inserida.|
| Solicitação de assinatura de certificado | Detalhes da Solicitação de assinatura de certificado (CSR), fornecidas pela autoridade de certificado. Detalhes do CSR não são necessários, mas devem ser fornecidos se forem parte do certificado. **Observação:** não mude o CSR de forma alguma. 
Uma chave pública pode ser incluída com o CSR e não deve ser substituída pela chave privada.|
|Comunicados | Quaisquer notas referentes ao certificado SSL que podem ser úteis para outros usuários.


## Próximas Etapas

Após a importação do certificado SSL para o {{site.data.keyword.slportal}}, ele será armazenado na tela
de certificados SSL até que seja [excluído manualmente](delete-ssl-certificate.html). Para todos os produtos ou
serviços que requerem detalhes do certificado SSL, o novo certificado SSL aparece na lista de certificados disponíveis para uso
ao interagir com o recurso SSL para o produto ou serviço procurado. O certificado pode ser
[atualizado](view-and-update-ssl-certificate.html) e os detalhes sobre o certificado podem ser
[transferidos por download com segurança](download-ssl-certificate-details.html) a qualquer momento.
