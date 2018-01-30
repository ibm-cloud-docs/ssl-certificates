---
copyright: years: 1994, 2017 lastupdated: "2017-11-30"
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

1. Acesse o [{{site.data.keyword.slportal}} ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://control.softlayer.com/){: new_window} usando suas credenciais exclusivas.
2. Selecione **Segurança > Certificados SSL >** para acessar a tela de certificados SSL.
3. Deve-se selecionar o tipo e a duração de certificado, envie o texto do CSR, preencha alguns detalhes adicionais e, em seguida, confirme o pagamento.

## Instalando e testando
Quando o processo de pedido e de validação for concluído, você receberá um e-mail da autoridade de certificação que incluiu seu certificado, bem como, todos os certificados intermediários.  O método para instalação desses certificados dependerá do software que você está usando, mas o resultado final deve ser o mesmo.  Quando terminar, você será capaz de visitar <http://host.yourdomain.com> e ver seu conteúdo enquanto vê também o cadeado SSL que os navegadores usam para denotar uma sessão criptografada.  Se você receber um aviso, deverá executar algumas etapas.

## Próximas Etapas

Após testar com sucesso, é possível acessar a tela de certificados SSL, para [atualizar](view-and-update-ssl-certificate.html), [fazer download](download-ssl-certificate-details.html), [excluir](delete-ssl-certificate.html) ou [importar](import-ssl-certificate.html) certificados SSL existentes na ferramenta.
