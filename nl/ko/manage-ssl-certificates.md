---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-12"

keywords: management of certificates, add certificate, managing certificates

subcollection: ssl-certificates

---

{:note: .note}
{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# SSL 인증서 관리
{: #managing-ssl-certificates}

{{site.data.keyword.cloud}} 콘솔에서 SSL 인증서를 관리할 수 있습니다. 인증서 관리 저장소 역할을 수행할 뿐 아니라 인증서를 사용하거나 필요한 서비스를 사용할 때도 필요합니다.

1. 콘솔의 보안 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)을 참조하십시오.
2. **보안** 메뉴에서 **SSL > 인증서 > 인증서 관리**를 선택하십시오.


현재 인증서 목록과 함께 해당 상태에 대한 정보가 제공됩니다.

인증서나 PEM 형식화된 버전을 검색하고 파트를 다운로드하거나 인증서 만기를 검토할 수 있습니다. 현재 각 인증서를 활용 중인 서비스 수도 볼 수 있습니다. 따라서 인증서의 만기일이 다가올 때 조치를 취해야 하는지 알 수 있습니다.

## 인증서 추가

인증서 추가가 준비되면 하위 탐색 메뉴에서 또는 인증서 목록 제목 내에서 **인증서 추가**를 선택하십시오. 인증서와 개인 키만 제공하면 됩니다. 그러나 발행자가 중간 인증서를 제공할 때 해당 인증서를 제공하지 않으면 인증서 체인이 중단되고 사용자 또는 관련 서비스의 유효성 검증이 적절하지 않게 될 수 있습니다.

비밀번호 문구가 필요한 개인 키는 저장할 수 없습니다.
{:note}

추가하고 나면 인증서에서 직접 다음 필드가 파생됩니다.

* 공통 이름
* 조직 이름
* 유효 기간

## 인증서 편집

인증서 왼쪽에 있는 삼각형을 활성화하면 인증서의 전체 파트가 표시됩니다. 따라서 인증서 파트를 편집할 수 있습니다. 참고를 추가할 수 있으며, 필요한 경우 인증서를 제거할 수 있습니다. 현재 인증서를 사용 중인 서비스 목록도 나열됩니다.

서비스와 연관되지 않은 인증서만 개인 키, 인증서 또는 중간 인증서 파트를 업데이트할 수 있습니다.  또한 인증서는 제거할 수 없습니다. 참고는 언제든 수정할 수 있습니다.

## 인증서 제거

인증서를 제거하려면 다음 단계를 따라 편집한 다음 "인증서 제거 확인"을 선택하고 저장하십시오.

## API 사용

API를 사용하여 인증서를 편집하는 예는 [SSL Management ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://sldn.softlayer.com/article/ssl-management){: new_window}를 참조하십시오.
