---
copyright:
  years: 1994, 2017
lastupdated: "2017-11-28"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 인증서 갱신

## 개요

{{site.data.keyword.BluSoftlayer_full}}를 통해 SSL 인증서를 주문하고 나면 언제든 갱신할 수 있습니다. 갱신 프로세스 중에 {{site.data.keyword.BluSoftlayer_notm}}는 고객(사용자)과 인증 기관 사이의 조정자 역할을 하며 SSL 인증서 세부사항이 필요한 갱신 프로세스의 일부를 보거나 제어하지 않습니다. SSL 인증서는 주문 당시 이용 약관이 동일하게 적용되어 갱신되므로 갱신 세부사항(예: 인증서 유형 및 권한, 유효한 달, 서버 플랫폼)을 변경할 수 없습니다. 인증서는 만기되기 전후에 갱신할 수 있습니다. 그러나 SSL 인증서의 유효성을 유지보수하려면 만기 날짜 이전에 인증서를 갱신하십시오. 아래 단계를 따라 SSL 인증서를 갱신하십시오.

## SSL 인증서 갱신

1. 고유 신임 정보를 사용하여 [{{site.data.keyword.slportal_full}} ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/){: new_window}에 액세스하십시오.
2. **보안** 메뉴에서 **SSL > 주문**을 선택하십시오.
3. 원하는 SSL 인증서의 **갱신** 열에서 **갱신** 링크를 클릭하십시오.

   **참고:** 요청을 완료하도록 팝업 창이 표시됩니다.  
   * 모든 갱신 및 CSR 세부사항이 올바른지 판별하십시오.<br /><br /><table border="1"><tr><th>상황</th><th>수행</th></tr><tr><td>모든 갱신 및 CSR 세부사항이 올바릅니다.</td><td>다음 단계로 진행하십시오. </td></tr><tr><td>갱신 세부사항이 잘못되었습니다.</td><td><ul><li>구매 화면으로 경로를 재지정할 <strong>새 SSL 인증서 구매</strong> 링크를 클릭하십시오.<br /><blockquote><strong>참고:</strong> 인증서 유형, 권한 및 이메일 승인 등의 갱신 세부사항을 변경할 수 없으므로 웹 사이트의 SSL 인증서에 대한 세부사항을 업데이트하는 유일한 방법은 새 인증서를 주문하는 것입니다.</blockquote></li><li>원하는 SSL 인증서 정보로 주문 페이지의 화면을 완료하십시오. 이 프로시저를 사용하면 추가 조치가 필요하지 않습니다.</li></ul></td></tr><tr><td>CSR 세부사항이 잘못되었습니다.</td><td><ul><li>**CSR 변경** 단추를 클릭하십시오.</li><li>**CSR** 텍스트 상자에서 **새 CSR 세부사항**을 입력하십시오.</li><li>**CSR 복원** 단추를 클릭하십시오.</li></ul></td></tr></table>
4. **갱신** 버튼을 클릭하여 SSL 인증서를 갱신하거나 **취소**를 클릭하여 조치를 취소하십시오.

## 다음 단계

SSL 인증서의 갱신을 요청하고 나면 {{site.data.keyword.BluSoftlayer_notm}}에서 갱신에 필요한 웹 사이트 검증을 완료하기 위해 인증 기관에 요청을 전달합니다. 인증서 갱신 시, 만기 필드에 새 만기 날짜가 표시됩니다.
