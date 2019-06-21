---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificate fulfillment email, fulfillment email

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 이행 이메일 요청
{: #requesting-an-ssl-certificate-fulfillment-email}

{{site.data.keyword.cloud}}를 통해 새 SSL 인증서를 주문하고 나면 인증 기관에서 주문 프로세스 중에 제공된 도메인 관리자에게 이행 이메일을 보냅니다. 이 이메일에는 SSL 인증서와 연관된 모든 세부사항이 포함되어 있습니다. {{site.data.keyword.cloud_notm}} 콘솔의 SSL 주문 화면에서 언제든 이행 이메일을 다시 요청할 수 있습니다. {:shortdesc}

## 이행 이메일 요청
다음 단계를 따라 인증 기관에서 SSL 이행 이메일을 요청하십시오.

1. 콘솔의 보안 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)을 참조하십시오.
2. **보안** 메뉴에서 **SSL > 주문**을 선택하십시오.
3. 원하는 SSL 인증서의 **이메일** 열에서 **보내기**를 클릭하십시오.

  팝업 창이 표시되어 요청을 확인합니다. 이 창에는 SSL 인증서를 요청할 때 제공된 도메인 관리자의 이메일 주소가 포함되어 있습니다.
{:note}

4. **이메일 다시 보내기**를 클릭하여 선택사항을 확인하고 인증 기관에서 추가 이행 이메일을 요청하십시오.

## 다음 단계

추가 이행 이메일을 요청하고 나면 완료를 위해 해당 인증 기관에 요청이 전달됩니다. SSL 인증서 세부사항은 기밀이므로 {{site.data.keyword.cloud_notm}}에서 시스템에 SSL 인증 데이터를 저장하지 않습니다. 이메일을 통해 SSL 인증서 세부사항을 받고 나면 필요한 경우 {{site.data.keyword.cloud_notm}} 콘솔에 수동으로 [가져오기](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)를 수행할 수 있습니다.
