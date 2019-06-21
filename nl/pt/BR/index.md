---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Tutorial de Introdução
{: #getting-started-tutorial}

## Antes
de Começar

A introdução ao SSL requer um pouco de planejamento. Conclua os pré-requisitos a seguir.

1. Decida onde obter o certificado
2. Saiba mais sobre os tipos de certificados, o comprimento da chave e a duração
3. Escolha um nome comum
4. Saiba mais sobre a regra do soquete
5. Gere o CSR

Para obter mais informações, consulte [Planejando para certificados SSL](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl).

## Solicitando certificados SSL

1. Navegue até o menu de segurança de seu console. Para obter mais informações, consulte [Navegando para dispositivos](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices).
2. No menu **Segurança**, selecione **Segurança > SSL > Certificados**.
3. Selecione **Pedir certificado SSL**.
3. Selecione o tipo e a duração de certificado, envie o texto da CSR, selecione a plataforma do servidor e, em seguida, confirme o pagamento.

## Instalando e testando
Após a conclusão do processo de pedido e de validação, você receberá um e-mail da autoridade de certificação que
inclui seu certificado, bem como todos os certificados intermediários necessários. O método para instalação depende do software que
você está usando, mas o resultado deve ser o mesmo. Quando terminar, você deverá ser capaz de acessar `http://host.yourdomain.com` e ver seu conteúdo e o cadeado de SSL que os navegadores usam para denotar uma sessão criptografada. Se você receber um aviso, deverá executar algumas etapas.

## Etapas seguintes

Após o teste bem-sucedido, é possível acessar os certificados SSL no console do {{site.data.keyword.cloud_notm}} para [atualizar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [fazer download](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [excluir](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) ou [importar](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) certificados SSL existentes no conjunto.
