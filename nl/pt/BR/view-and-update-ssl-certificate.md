---
copyright:
  years: 2014, 2018
lastupdated: "2018-08-15"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizando e atualizando certificados SSL

Após a importação de um certificado SSL para a tela de certificados SSL, é possível visualizá-los e atualizá-los a
qualquer momento. As atualizações funcionam de forma semelhante ao [processo de importação](import-ssl-certificate.html), pois todos os detalhes atualizados devem corresponder exatamente ao certificado original, incluindo espaçamentos e quebras de linha.

Para visualizar e atualizar um certificado SSL, conclua as etapas a seguir.

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados**.
2. Selecione **Visualizar/Atualizar certificado** na lista suspensa **Ações**.
3. Atualize os **Detalhes do certificado SSL** nas caixas de texto aplicáveis.

   **Nota:** detalhes que são inseridos na janela **Importar certificado SSL** devem ser
inseridos exatamente como fornecidos pela autoridade de certificação, incluindo espaçamento e quebras de linha. Se não, ocorre um erro.

|Detalhes do certificado SSL  | Descrição |
| --------------------------- | ----------- |
|Certificado                  | Detalhes do certificado SSL, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Chave privada                  | Detalhes da chave privada para o certificado, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Certificado intermediário     | Detalhes do certificado intermediário, fornecidos pela autoridade de certificação. Certificados intermediários não são necessários, no entanto, se a informação estiver disponível para o certificado SSL, ela deve ser inserida.|
|Solicitação de assinatura de certificado  | Detalhes da Solicitação de assinatura de certificado (CSR), fornecidas pela autoridade de certificado. Detalhes do CSR não são necessários, mas devem ser fornecidos se forem parte do certificado. **Observação:** não mude o CSR de forma alguma. Uma chave pública pode ser incluída com o CSR e não deve ser substituída pela chave privada.|
|Comunicados                        | Quaisquer notas referentes ao certificado SSL que podem ser úteis para outros usuários.|
{: caption="Tabela 1. Detalhes do certificado SSL" caption-side="top"}

Clique em **Atualizar** para atualizar o certificado SSL ou clique em **Cancelar** para cancelar a ação.

## Próximas Etapas

Após atualizar os detalhes para o certificado SSL, quaisquer produtos ou serviços que usam o certificado não serão impactados negativamente pela mudança. O certificado pode ser atualizado novamente a qualquer momento repetindo as etapas anteriores.
