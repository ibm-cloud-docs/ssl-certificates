---

copyright:
  years: 2014, 2018
lastupdated: "2018-05-17"

keywords: PPTP VPN access, PPTP VPN, PPTP access

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# PPTP VPN 액세스 활성화 또는 비활성화
{: #activating-or-deactivating-pptp-vpn-access}

PPTP VPN을 사용하면 데스크탑 또는 전용 디바이스에서 실행 중인 특수 클라이언트 소프트웨어를 사용하여 {{site.data.keyword.BluSoftlayer_full}} 사설 네트워크에 대한 보안 터널을 형성할 수 있습니다. PPTP 액세스는 전체 사무실에 연결해야 하거나 SSL VPN 솔루션을 사용할 수 없는 고객용으로 설계되었습니다. 각 고객에게는 추가로 연결이 사용 가능하지만 무제한 PPTP 액세스(추가 비용 없이 사용 가능함)를 사용하려면 지원이 필요한 하나의 PPTP 연결이 할당됩니다. 사용자의 PPTP VPN 액세스를 활성화하거나 비활성화하려면 다음 단계를 완료하십시오.

1. 관리자로서 고유 인증 정보를 사용하여 [{{site.data.keyword.slportal_full}} ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/){: new_window}에 액세스하십시오.
2. 액세스 권한을 수정할 사용자를 찾아 **VPN 액세스** 열을 보고 현재 액세스 레벨을 확인하십시오.
3. **조치** 메뉴에서 **VPN 액세스 편집**을 선택하십시오.
4. VPN 유형과 서브넷 액세스 세부사항을 입력하십시오.

|필드 이름  |옵션   |
| -----------| ------------ |
|VPN 유형   |없음, SSL, PPTP 또는 둘 다(SSL 및 PPTP) |
|서브넷 액세스 |자동 또는 수동 |           
{: caption="표 1. VPN 및 서브넷 세부사항" caption-side="top"}   
5. **저장**을 클릭하여 변경사항을 저장하십시오.

   **참고:** 사용자가 PPTP를 사용하여 연결하려면 PPTP 액세스를 활성화해야 합니다.
