---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"

keywords: SSL certificates FAQ, SSL FAQ

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:faq: data-hd-content-type='faq'}

<a name="top"></a>
# FAQ: SSL 인증서
{: #faqs-ssl-certificates}

## 주문한 SSL 인증서가 SSL 인증서 화면에 자동으로 표시되지 않는 이유는 무엇입니까?
{:faq}

SSL 인증서는 서드파티 인증 기관에서 발행되며, 이 기관에서는 모든 인증서 세부사항을 기밀 이메일로 사용자에게 직접 전송합니다. {{site.data.keyword.BluSoftlayer_full}} 제품 및 서비스와 인증서를 사용하도록 선택하는 경우 이 이메일을 받고 나면 {{site.data.keyword.slportal_full}}에 [SSL 인증서 가져오기](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates) 옵션이 있습니다. {{site.data.keyword.cloud_notm}}에서 SSL 인증서의 세부사항을 받지 못하므로 데이터를 자동으로 가져올 수 없습니다.

## SSL 인증서란 무엇입니까?
{:faq}

SSL 인증서는 사용자를 보호하는 보안 조치로 웹 사이트에서 사용됩니다. 일반적으로 이름, 주소, 신용카드 번호 및 기타 개인 데이터 등의 기밀 정보를 웹 사이트에 전송해야 하거나 인증이 필요한 데이터를 관리하는 경우(예: {{site.data.keyword.slportal}}에서) 인증서가 사용됩니다. SSL 인증서는 웹 사이트를 실행하는 회사에서 요청하지만, 발행은 웹 사이트의 유효성을 확인하는 신뢰할 수 있는 서드파티 회사에서 수행합니다. 표준 HTTP와 달리 보안 웹 사이트는 URL 앞에 HTTPS가 옵니다.

## SHA2 SSL은 어떻게 주문합니까?
{:faq}

이미 SSL을 주문했으며 SSL 인증서에서 SHA-2가 아니라 SHA-1을 사용하고 있다는 오류를 표시하면 SSL을 다시 발행하도록 요청해야 합니다. 이 작업은 티켓을 제출하여 수행할 수 있습니다.

{{site.data.keyword.cloud_notm}}에서 아직 SSL을 주문하지 않았으며 SHA-2를 사용하는 SSL을 주문해야 하는 경우 문제의 도메인에 대한 SSL을 수동으로 주문하기 위해 티켓을 제출하십시오. {{site.data.keyword.slportal}}에서는 여전히 SHA-1을 사용하여 SSL 인증서를 자동으로 작성하므로, 이 작업을 수행하는 경우 인증서를 다시 발행해야 합니다.
