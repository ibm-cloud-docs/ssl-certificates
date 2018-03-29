---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-21"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introdução aos certificados SSL  


## Antes
de Começar

A introdução ao SSL requer um pouco de planejamento. Conclua os pré-requisitos a seguir.

1. Decida onde obter o certificado
2. Saiba mais sobre os tipos de certificados, o comprimento da chave e a duração
3. Escolha um nome comum
4. Saiba mais sobre a regra do soquete
5. Gere o CSR

Para obter mais informações, consulte [Planejando para certificados SSL](planning-ahead-ssl.html).

## Solicitando certificados SSL

1. Acesse o [{{site.data.keyword.slportal_full}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. Selecione **Segurança > Certificados SSL >** para acessar a tela de certificados SSL.
3. Deve-se selecionar o tipo e a duração de certificado, enviar o texto do CSR, inserir alguns detalhes adicionais e,
em seguida, confirmar o pagamento.

## Instalando e testando
Após a conclusão do processo de pedido e de validação, você receberá um e-mail da autoridade de certificação que
inclui seu certificado, bem como todos os certificados intermediários necessários. O método para instalação depende do software que
você está usando, mas o resultado deve ser o mesmo. Quando terminado, você será capaz de acessar o
<http://host.yourdomain.com> e ver seu conteúdo, além de ver o cadeado SSL que os navegadores usam para denotar uma sessão criptografada. Se você receber um aviso, deverá executar algumas etapas.

## Próximas Etapas

Após testar com sucesso, é possível acessar a tela de certificados SSL, para [atualizar](view-and-update-ssl-certificate.html), [fazer download](download-ssl-certificate-details.html), [excluir](delete-ssl-certificate.html) ou [importar](import-ssl-certificate.html) certificados SSL existentes na ferramenta.
