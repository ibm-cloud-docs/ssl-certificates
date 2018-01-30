---
copyright: years: 1994, 2017 lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Instalando certificados SSL no Plesk 9

Para incluir certificados SSL no Plesk 9, conclua as etapas a seguir.

1. Efetue login no Plesk e navegue para o domínio no qual você deseja instalar o certificado.
2. Entre na configuração do domínio de destino.
3. Clique em **certificados SSL**.
4. Clique em **Incluir certificado SSL**.

   **Observação:** se você já possuir um certificado SSL, ignore esta etapa e vá para a 8.
5.  Nomeie o certificado.  É possível nomeá-lo como qualquer coisa, mas pode ser útil usar um nome descritivo, incluindo um registro de data e hora.

   Nesse caso, estamos usando o formato *YYYYMMDDRR*, em que *RR* é o número da revisão (00, neste caso, pois não há revisões para o mesmo dia).
6. Faça quaisquer ajustes necessários para a solicitação SSL. Essas informações serão integradas no certificado SSL e devem ser semelhantes às informações de registro do domínio.

  O endereço de e-mail deve corresponder a um dos endereços de e-mail no domínio cujas informações foram fornecidas pelo escrivão de domínio.

  **Importante:** informações falsas podem ser rejeitadas por sua autoridade de certificação SSL.
7. Navegue de volta para a configuração do certificado.
8. Revise o CSR e a chave privada e salve a chave privada em um local seguro.  

  **Observação:** se algo ocorrer com o servidor de modo que o certificado tenha que ser inserido novamente, você deverá ter pelo menos o certificado e chave privada.
9. Pegue o CSR e envie-o para a autoridade de certificação de sua escolha. A infraestrutura do {{site.data.keyword.cloud_notm}} não fornece certificados SSL.
10. Depois de receber o certificado de sua autoridade de certificação, é possível colá-lo na área de texto do certificado.

   **Notas:**
   * Se a autoridade de certificação exigir, você poderá precisar colar seu próprio certificado na área de texto do certificado de autoridade de certificação (geralmente chamado de Pacote configurável de certificado de autoridade de certificação).
   * Deve-se ter uma chave privada e um certificado correspondente para usar um certificado.
11. Navegue de volta para as *<span style="text-decoration: underline">Configurações de hospedagem da web</span>* na configuração de Domínios.
12. Selecione o certificado correspondente e clique em **OK**.

O novo certificado agora está sendo usado para o domínio.  Se você atualizar o certificado, poderá ser necessário fechar completamente o navegador antes de usar o novo certificado.
