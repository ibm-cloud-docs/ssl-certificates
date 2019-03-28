---

copyright:
  years: 2014, 2018
lastupdated: "2018-06-20"

keywords: importing SSL certificates,SSL import, SSL certificate details

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 인증서 가져오기
{: #importing-ssl-certificates}

웹 사이트의 SSL 인증서를 발생한 다음 {{site.data.keyword.slportal_full}}로 가져올 수 있습니다. SSL 인증서를 {{site.data.keyword.slportal}}에 가져와서 인증서가 필요한 제품과 서비스에 적용할 수 있습니다(예: 로드 밸런서의 [SSL 오프로딩](/docs/infrastructure/local-load-balancer?topic=local-load-balancer-configuring-ssl-offloading-on-a-load-balancer)). 기본적으로 {{site.data.keyword.BluSoftlayer_full}}에서 발행한 SSL 인증서는 수신인만 조작할 수 있으므로 목록에 가져오지 않습니다. 따라서 {{site.data.keyword.BluSoftlayer_notm}} 제품 또는 서비스와 함께 사용할 SSL 인증서는 계정에 대해 인증된 사용자가 수동으로 가져와야 합니다. 다음 단계를 완료하여 SSL 인증서를 {{site.data.keyword.slportal}}에 가져오십시오.

1. 고유 인증 정보를 사용하여 [{{site.data.keyword.slportal_full}} ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/){: new_window}에 액세스하십시오.
2. **보안** 메뉴에서 **SSL > 인증서**를 선택하십시오.
3. **SSL 인증서 가져오기**를 클릭하십시오.
4. 해당 필드에 **SSL 인증서 세부사항**을 입력하고 **가져오기**를 클릭하십시오.

   **참고:** **SSL 인증서 가져오기** 창에 입력한 세부사항은 간격과 행 바꾸기를 포함하여 인증 기관에서 제공한 내용과 똑같이 입력해야 합니다. 그렇지 않으면 오류가 발생합니다.

| SSL 인증서 세부사항     |설명 |
| --------------------------- | ----------- |
|인증서                  |인증 기관에서 제공한 SSL 인증서 세부사항입니다. 일반적으로 텍스트의 영숫자 블록입니다.|
|개인 키                  |인증 기관에서 제공한 인증서의 개인 키 세부사항입니다. 일반적으로 텍스트의 영숫자 블록입니다.|
|중간 인증서     |인증 기관에서 제공한 중간 인증서 세부사항입니다. 중간 인증서는 필수가 아니지만, SSL 인증서의 정보를 사용할 수 있으면 입력해야 합니다.|
|인증서 서명 요청  |인증 기관에서 제공한 인증서 서명 요청(CSR)입니다. CSR 세부사항은 필수가 아니지만 인증서의 파트인 경우 제공해야 합니다. **참고:** 어떤 식으로든 CSR을 변경하지 마십시오. 공개 키는 CSR에 포함될 수 있으며 개인 키로 바꾸지 않아야 합니다.|
|참고                        |다른 사용자에게 유용할 수 있는 SSL 인증서와 관련된 참고사항입니다.|
{: caption="표 1. SSL 인증서 세부사항" caption-side="top"}

## 다음 단계

SSL 인증서를 {{site.data.keyword.slportal}}에 가져오고 나면 [수동으로 삭제](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates)할 때까지 SSL 인증서 화면에 저장됩니다. SSL 인증서 세부사항이 필요한 모든 제품 또는 서비스의 경우 원하는 제품 또는 서비스를 위해 SSL 기능과 상호작용할 때 사용할 수 있는 인증서 목록에 새로운 SSL 인증서가 표시됩니다. 인증서는 [업데이트](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates)할 수 있으며 인증서에 대한 세부사항은 언제든 [안전하게 다운로드](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details)할 수 있습니다.
