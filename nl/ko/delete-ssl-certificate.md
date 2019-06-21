---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: SSL certificates delete, SSL delete

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 인증서 삭제
{: #deleting-ssl-certificates}

SSL 인증서 세부사항을 {{site.data.keyword.cloud}} 콘솔에 가져오고 나면 {{site.data.keyword.cloud_notm}}에 저장된 모든 데이터를 제거하기 위해 언제든 해당 세부사항을 삭제할 수 있습니다.

SSL 인증서를 삭제하려면 다음 단계를 완료하십시오.

1. 콘솔의 보안 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)을 참조하십시오.
2. **보안** 메뉴에서 **SSL > 인증서**를 선택하십시오.
3. **조치** 메뉴에서 원하는 SSL 인증서에 대해 **삭제**를 선택하십시오.
4. **예**를 클릭하여 SSL 인증서를 삭제하십시오.

## 다음 단계

SSL 인증서를 삭제하고 나면 인증서에 연결된 모든 서비스가 더 이상 해당 정보를 이용하지 않습니다. {{site.data.keyword.cloud_notm}} 콘솔의 SSL 인증서 화면에 더 이상 인증서가 표시되지 않습니다.

삭제된 인증서를 이전에 사용한 모든 서비스가 계정과 연관된 올바른 SSL 인증서와 연관되도록 모든 서비스를 업데이트하십시오. 

[가져오기](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates) 프로세스를 사용하여 언제든 SSL 인증서를 {{site.data.keyword.cloud_notm}} 콘솔에 다시 추가할 수 있습니다.{:note}
