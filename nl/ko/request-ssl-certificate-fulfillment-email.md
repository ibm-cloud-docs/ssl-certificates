---
copyright:
  years: 2014, 2018
lastupdated: "2018-02-22"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 이행 이메일 요청

{{site.data.keyword.BluSoftlayer_full}}를 통해 새 SSL 인증서를 주문하고 나면 인증 기관에서 주문 프로세스 중에 제공된 도메인 관리자에게 이행 이메일을 보냅니다. 이 이메일에는 SSL 인증서와 연관된 모든 세부사항이 포함되어 있습니다. {{site.data.keyword.slportal_full}}의 SSL 주문 화면에서 언제든 이행 이메일을 다시 요청할 수 있습니다. 다음 단계를 따라 인증 기관에서 SSL 이행 이메일을 요청하십시오.

## 이행 이메일 요청

1. 고유 신임 정보를 사용하여 [{{site.data.keyword.slportal_full}} ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/){: new_window}에 액세스하십시오.
2. **보안** 메뉴에서 **SSL > 주문**을 선택하십시오.
3. 원하는 SSL 인증서의 **이메일** 열에서 **보내기** 링크를 클릭하십시오.<br/>**참고:** 팝업 창이 표시되어 요청을 확인합니다. 이 창에는 SSL 인증서를 요청할 때 제공된 도메인 관리자의 이메일 주소가 포함되어 있습니다.
4. **이메일 다시 보내기**를 클릭하여 선택사항을 확인하고 인증 기관에서 추가 이행 이메일을 요청하십시오.  또는 **취소**를 클릭하여 조치를 취소하십시오.

## 다음 단계

추가 이행 이메일을 요청하고 나면 완료를 위해 해당 인증 기관에 요청이 전달됩니다. SSL 인증서 세부사항은 기밀이므로 {{site.data.keyword.BluSoftlayer_notm}}에서 시스템에 SSL 인증 데이터를 저장하지 않습니다. 이메일을 통해 SSL 인증서 세부사항을 받고 나면 필요한 경우 {{site.data.keyword.slportal}}에 수동으로 [가져오기](import-ssl-certificate.html)를 수행할 수 있습니다.
