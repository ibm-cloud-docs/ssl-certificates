---
copyright: years: 1994, 2017 lastupdated: "2017-11-30"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introdução à tecnologia de SSL

Secure Sockets Layer (SSL) é uma tecnologia que criptografa o tráfego entre o aplicativo cliente e o aplicativo do servidor. Essa criptografia é realizada usando um sistema de chave pública/chave privada usando um certificado SSL.

O certificado SSL contém a chave pública do servidor, as datas para as quais o certificado é válido, um nome de host para o qual o certificado é válido e uma assinatura da autoridade de certificação que a emitiu.

## Terminologia SSL

Certificados SSL têm terminologia exclusiva. Você pode encontrar os termos a seguir ao trabalhar com certificados SSL.

**Tamanho de bit:** chaves de criptografia são medidas por seu tamanho em bits. Por exemplo 512 bits, 1024 bits, 2048 bits. Geralmente, uma chave mais longa será mais segura, mas mais lenta quanto ao uso. Nesse momento, o tamanho mínimo para as chaves usadas em certificados SSL é 1024 bits, embora os certificados de Validação Estendida requerem 2048 bits.

**Cadeia de certificados:** os certificados SSL geralmente não são utilizados sozinhos. Na maioria das implementações você estará lidando com uma cadeia de certificados. Por exemplo:

  Root > intermediate1 > server cert.

  \> Intermediate2 > server2 cert

Nesse exemplo, seu certificado do servidor é assinado pelo certificado intermediário, que é, por sua vez, assinado pelo certificado raiz. O encadeamento dessa maneira pode tornar o SSL mais seguro porque significa que o certificado raiz não é usado (e exposto ao risco) frequentemente. Se o intermediate1 for comprometido, o certificado do servidor poderá estar em danificado, mas o certificado do servidor 2 deverá estar bom porque eles fazem parte de cadeias diferentes.

**Solicitação de assinatura de certificado:** o CSR é um documento que você gera no servidor que contém informações que a autoridade de certificação usa para criar seu certificado real.

**Nome comum:** o Nome Comum (CN) é o nome do host para o qual o certificado é válido (por exemplo, www.domain.com).  

*Observação:* www.domain.com, smtp.domain.com e mail.domain.com são três nomes de host completamente diferentes e o mesmo certificado SSL não é válido para todos os três (a menos que você esteja usando um certificado curinga, mas, neste momento, o {{site.data.keyword.cloud}} não os oferece).

**Chave privada/chave pública:** o SSL faz uso de uma técnica chamada criptografia de chave pública. Nessa forma de criptografia, você tem duas chaves: a pública e a privada. A chave pública está distribuída por toda parte. Ninguém vê sua chave privada. Pessoas que desejam se comunicar de forma segura com você criptografam suas comunicações usando sua chave pública. A criptografia de chave pública é baseada na afirmação de que os bits criptografados com uma determinada chave pública só podem ser descriptografados usando a chave privada correspondente e vice-versa.

**Certificado raiz:** os certificados raiz SSL são certificados que foram assinados e apresentados ao mundo por suas respectivas Autoridades de Certificação como o topo de sua cadeia. Você encontrará certificados raiz para Autoridades de Certificação já instalados no armazenamento de certificados para seu navegador da web. Isso permite que seu navegador confie nesses certificados e seja o começo da cadeia de confiança que leva ao certificado que você instalou em seu servidor.

**Assinatura:** os certificados SSL têm uma assinatura digital colocada sobre eles pela autoridade de certificação. Essa assinatura, quando rastreada de volta para um certificado raiz confiável, confirma a autenticidade do certificado.

## SSL na infraestrutura do IBM Cloud

O {{site.data.keyword.BluSoftlayer_full}} revende três tipos de certificados SSL: a Validação de domínio, a Validação de organização e a Validação estendida. 

Os certificados de Validação de Domínio (DV) são baratos e disponíveis rapidamente. A validação feita pela Autoridade de Certificação está limitada ao envio de um e-mail para um endereço de e-mail especificado no domínio em questão e ao recebimento de uma resposta positiva. Os certificados de Validação de Organização (OV) e de Validação Estendida (EV) levam alguns dias (às vezes uma semana), custam mais e resultam em mais verificações pela Autoridade de Certificação. Os certificados EV são codificados de forma que os navegadores os reconheçam como EV e geralmente exibem uma barra verde como parte da barra de endereços. 

Os certificados SSL, como outros serviços do {{site.data.keyword.cloud_notm}}, podem ser gerenciados por meio do {{site.data.keyword.slportal}}.  Acesse o menu **Segurança** e selecione a opção **Certificados SSL** na parte inferior para solicitar e gerenciar certificados.  

**Observação:** os certificados SSL ordenados por meio de {{site.data.keyword.cloud_notm}} não devem ser utilizados em um servidor {{site.data.keyword.BluSoftlayer_notm}}. Além disso, os certificados ordenados em outro local podem ser usados em seus servidores hospedados aqui.

**Conclusão**

Os certificados SSL aprimoram a segurança das transações que estão ocorrendo e dão aos usuários um senso de segurança. Além dos certificados SSL, a segurança Daemon, a segurança física, as práticas de codificação e o gerenciamento de certificados combinam-se para formar o perfil geral de segurança da solução.
