---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords:  renewing SSL certificates, renewal SSL, SSL certificate renewal process, renewing, renewal

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 인증서 갱신
{: #renewing-ssl-certificates}

{{site.data.keyword.cloud}}를 통해 SSL 인증서를 주문하고 나면 언제든 갱신할 수 있습니다. 갱신 프로세스 중에 {{site.data.keyword.cloud_notm}}는 사용자와 인증 기관 사이의 조정자 역할을 하며, SSL 인증서 세부사항이 포함된 갱신 프로세스의 일부를 보거나 제어하지 않습니다. SSL 인증서는 주문 당시 이용 약관이 동일하게 적용되어 갱신되므로 갱신 세부사항(예: 인증서 유형 및 권한, 유효한 달, 서버 플랫폼)을 변경할 수 없습니다. 인증서는 만기되기 전후에 갱신할 수 있습니다. 그러나 SSL 인증서의 유효성을 유지보수하려면 만기 날짜 이전에 인증서를 갱신하십시오.
{:shortdesc}

## SSL 인증서 갱신
다음 단계를 완료하여 SSL 인증서를 갱신하십시오.

1. 콘솔의 보안 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)을 참조하십시오.
2. **보안** 메뉴에서 **SSL > 주문**을 선택하십시오.
3. 원하는 SSL 인증서의 **갱신** 열에서 **갱신**을 클릭하십시오.
4. SSL 인증서를 갱신하기 전에 모든 갱신 및 CSR 세부사항이 올바른지 판별하십시오. 자세한 정보는 다음 표를 참조하십시오.   

| 세부사항                        | 조치    |
| ------------------------------- | ------- |
| 올바른 갱신 및 CSR 세부사항     | **갱신**을 선택하여 SSL 인증서를 갱신하십시오. |
| 올바르지 않은 갱신 세부사항     | **새 SSL 인증서 구매**를 선택하여 새 인증서를 주문하십시오. 인증서 유형, 권한 및 이메일 승인 등의 갱신 세부사항을 변경할 수 없으므로 웹 사이트의 SSL 인증서에 대한 세부사항을 업데이트하는 유일한 방법은 새 인증서를 주문하는 것입니다.|
| 올바르지 않은 CSR 세부사항      | **CSR 변경**을 선택하고, **CSR 텍스트 상자**에 새 CSR 세부사항을 입력하고, **CSR 복원**을 선택하십시오. |
{: caption="표 1. 갱신 및 CSR 세부사항" caption-side="top"}

## 다음 단계

SSL 인증서의 갱신을 요청하고 나면 {{site.data.keyword.cloud_notm}}에서 갱신에 필요한 웹 사이트 검증을 완료하기 위해 인증 기관에 요청을 전달합니다. 인증서 갱신 시 **만기** 필드에 새 만기 날짜가 표시됩니다.
