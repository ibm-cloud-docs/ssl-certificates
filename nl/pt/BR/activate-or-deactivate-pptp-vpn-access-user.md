---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:external: target="_blank" .external}

# Ativando ou desativando o acesso VPN PPTP
{: #activating-or-deactivating-pptp-vpn-access}

A VPN PPTP permite que você forme um túnel seguro até a rede privada do {{site.data.keyword.cloud}} usando um software cliente especializado que é executado em sua área de trabalho ou em seu dispositivo dedicado. O acesso PPTP será projetado se você precisar conectar um escritório inteiro ou não puder usar a solução VPN SSL. Uma conexão PPTP com mais conexões disponíveis é alocada para você e é possível solicitar suporte para ativar o acesso PPTP ilimitado, que está disponível sem encargo adicional. Para ativar ou desativar o acesso VPN PPTP para um usuário, conclua as etapas a seguir.
{:shortdesc}

1. Efetue login na página [Acesso (IAM)](https://cloud.ibm.com/iam/overview){: external} no console do {{site.data.keyword.cloud_notm}}.
2. Localize o usuário cujo acesso você gostaria de modificar e visualize a coluna **Acesso VPN** para visualizar seu nível atual de acesso.
3. No menu **Ações**, selecione **Editar acesso VPN**.
4. Insira os detalhes de tipo de VPN e de acesso de sub-rede e clique em **Salvar** para salvar suas mudanças. Consulte a tabela a seguir para obter informações adicionais.

|Nome de Campo  |Opções   |
| -----------| ------------ |
| Tipo de VPN   | Nenhum, SSL, PPTP ou ambos (SSL e PPTP) |
| Acesso à sub-rede | Automático ou manual |           
{: caption="Tabela 1. Detalhes da VPN e da sub-rede" caption-side="top"}   

O acesso PPTP deve ser ativado para que um usuário se conecte usando PPTP.
{:note}
