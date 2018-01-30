---
copyright: years: 1994, 2017 lastupdated: "2017-11-17"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Visualizando e atualizando certificados SSL

Após um certificado SSL ter sido importado para a tela de certificados SSL, será possível visualizá-lo e atualizá-lo a qualquer momento. As atualizações funcionam de forma semelhante ao [processo de importação](import-ssl-certificate.html), pois todos os detalhes atualizados devem corresponder exatamente ao certificado original, incluindo espaçamentos e quebras de linha.

Para visualizar e atualizar um certificado SSL, conclua as etapas a seguir.

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. No menu **Segurança**, selecione **SSL > Certificados**.
2. Selecione **Visualizar/Atualizar certificado** na lista suspensa **Ações**.
3. Atualize os **Detalhes do certificado SSL** nas caixas de texto aplicáveis.

   **Observação:** os detalhes inseridos na janela **Importar certificado SSL** devem ser inseridos exatamente como fornecidos pela autoridade de certificação, incluindo espaçamento e quebras de linha. Se não, ocorre um erro.

| Caixa de texto | Entrada |
| -------- | ----- |
|Certificado |Detalhes do certificado SSL, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Chave privada | Detalhes da chave privada para o certificado, fornecidos pela autoridade de certificação. Geralmente é um bloco alfanumérico de texto.|
|Certificado intermediário | Detalhes do certificado intermediário, fornecidos pela autoridade de certificação. Certificados intermediários não são necessários, no entanto, se a informação estiver disponível para o certificado SSL, ela deve ser inserida.|
| Solicitação de assinatura de certificado | Detalhes da Solicitação de assinatura de certificado (CSR), fornecidas pela autoridade de certificado. Detalhes do CSR não são necessários, mas devem ser fornecidos se forem parte do certificado. **Observação:** não mude o CSR de forma alguma. Uma chave pública pode ser incluída no CSR e não deve ser substituída pela Chave Privada.|
|Comunicados | Quaisquer notas sobre o certificado SSL que possam ser úteis para outros usuários.
Clique em **Atualizar** para atualizar o certificado SSL ou clique em **Cancelar** para cancelar a ação.

## Próximas Etapas

Após atualizar os detalhes para o certificado SSL, quaisquer produtos ou serviços que usam o certificado não serão impactados negativamente pela mudança. O certificado pode ser atualizado novamente a qualquer momento, repetindo as etapas acima.
