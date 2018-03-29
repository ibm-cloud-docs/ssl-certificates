---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Ativando ou desativando o acesso VPN PPTP

A VPN PPTP permite que os usuários formem um túnel seguro para a rede privada do {{site.data.keyword.BluSoftlayer_full}} usando software cliente especializado que é executado em sua área de trabalho ou dispositivo dedicado. O acesso PPTP é projetado para clientes que precisam conectar um escritório inteiro ou que não podem usar a solução VPN SSL. A cada cliente é atribuído uma conexão PPTP com conexões adicionais disponíveis, mas solicitando suporte para ativar o acesso PPTP ilimitado, que está disponível sem custo adicional. Para ativar ou desativar o acesso VPN PPTP para um usuário, conclua as etapas a seguir.

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas como um administrador.
2. Localize o usuário cujo acesso você gostaria de modificar e visualize a coluna **Acesso VPN** para visualizar seu nível atual de acesso.
3. No menu **Ações**, selecione **Editar acesso VPN**.
4. Insira o tipo VPN e os detalhes de acesso de sub-rede.

|Nome de Campo  |Opções   |
| -----------| ------------ |
| Tipo de VPN   | Nenhum, SSL, PPTP ou ambos (SSL e PPTP) |
|Acesso à sub-rede | Automático ou manual |           
{: caption="Tabela 1. Editar opções de acesso VPN" caption-side="top"}   
5. Clique em **Salvar** para salvar suas mudanças.

   **Nota:** o acesso PPTP deve ser ativado para que um usuário se conecte usando PPTP.
