---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: view SSL certificates, update SSL certificates, original certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizando e atualizando certificados SSL
{: #viewing-and-updating-ssl-certificates}

Depois que um certificado SSL é importado para a tela Certificados SSL, é possível visualizá-lo e atualizá-lo a qualquer momento. As atualizações funcionam de forma semelhante ao [processo de importação](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates), pois todos os detalhes atualizados devem corresponder exatamente ao certificado original, incluindo espaçamentos e quebras de linha.
{:shortdesc}

Para visualizar e atualizar um certificado SSL, conclua as etapas a seguir.

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **SSL > Certificados**.
3. Selecione **Visualizar/Atualizar certificado** na lista suspensa **Ações**.
4. Atualize os **Detalhes do certificado SSL** nas caixas de texto aplicáveis e clique em **Atualizar** para aplicar suas mudanças. Consulte a tabela a seguir para obter informações adicionais.

   Os detalhes que são inseridos na janela **Importar certificado SSL** devem ser inseridos exatamente conforme fornecidos pela autoridade de certificação, incluindo espaçamento e quebras de linha. Se não, ocorre um erro.
   {:note}

| Detalhes do certificado SSL     | Descrição |
| --------------------------- | ----------- |
|Certificado                  | Detalhes do certificado SSL que são fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Chave privada                  | Detalhes da chave privada para o certificado que são fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|certificado intermediário     | Detalhes do certificado intermediário que são fornecidos pela autoridade de certificação. Os certificados intermediários não são necessários. Porém, se as informações estiverem disponíveis para o certificado SSL, elas deverão ser inseridas.|
|Solicitação de assinatura de certificado  | Detalhes da solicitação de assinatura de certificado (CSR) que são fornecidos pela autoridade de certificação. Detalhes do CSR não são necessários, mas devem ser fornecidos se forem parte do certificado. **Observação:** não mude o CSR de forma alguma. Uma chave pública pode ser incluída com a CSR e não deve ser substituída pela chave privada.|
|Comunicados                        | Quaisquer notas referentes ao certificado SSL que podem ser úteis para outros usuários.|
{: caption="Tabela 1. Detalhes do certificado SSL" caption-side="top"}

## Etapas seguintes

Após atualizar os detalhes para o certificado SSL, quaisquer produtos ou serviços que usam o certificado não serão impactados negativamente pela mudança. O certificado pode ser atualizado novamente a qualquer momento repetindo as etapas anteriores.
