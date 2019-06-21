---

copyright:
  years: 2014, 2019
lastupdated: "2019-06-11"

keywords: types of certificates,SSL certificates, Select Security

subcollection: ssl-certificates

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 시작하기 튜토리얼
{: #getting-started-tutorial}

## 시작하기 전에

SSL을 시작하려면 플랜 비트가 필요합니다. 다음 전제조건을 완료하십시오.

1. 인증서를 가져올 위치 결정
2. 인증서 유형, 키 길이 및 기간에 대해 학습
3. 공통 이름 선택
4. 소켓 규칙 학습
5. CSR 생성

자세한 정보는 [SSL 인증서 플랜](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-planning-for-ssl#planning-for-ssl)을 참조하십시오.

## SSL 인증서 주문

1. 콘솔의 보안 메뉴로 이동하십시오. 자세한 정보는 [디바이스로 이동](/docs/infrastructure/ssl-certificates?topic=virtual-servers-navigating-devices)을 참조하십시오.
2. **보안** 메뉴에서 **보안 > SSL > 인증서**를 선택하십시오.
3. **이전 SSL 인증서**를 선택하십시오.
3. 인증서의 유형과 기간을 선택하고, CSR의 텍스트를 제출한 다음, 서버 플랫폼을 선택하고, 결제를 확인하십시오. 

## 설치 및 테스트
주문 및 유효성 검증 프로세스가 완료되고 나면 인증서 외에도 필수 중간 인증서를 포함하는 인증 기관에서 이메일을 받습니다. 설치 방법은 사용 중인 소프트웨어에 따라 다르지만 결과는 같아야 합니다. 완료되면 `http://host.yourdomain.com`으로 이동할 수 있어야 하고, 브라우저에서 암호화된 세션을 나타내는 데 사용하는 SSL 패드락이 표시되는 동안 컨텐츠도 볼 수 있어야 합니다. 경고를 받으면 수행해야 하는 단계가 있습니다.

## 다음 단계

성공적으로 테스트하고 나면 {{site.data.keyword.cloud_notm}} 콘솔의 SSL 인증서에 액세스하여 기존 SSL 인증서를 [업데이트](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-viewing-and-updating-ssl-certificates#viewing-and-updating-ssl-certificates), [다운로드](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-downloading-ssl-certificate-details#downloading-ssl-certificate-details), [삭제](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-deleting-ssl-certificates#deleting-ssl-certificates) 또는 도구에 [가져오기](/docs/infrastructure/ssl-certificates?topic=ssl-certificates-importing-ssl-certificates#importing-ssl-certificates)를 수행할 수 있습니다.
