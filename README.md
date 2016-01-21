# Security Best Practices

인터넷으로 서비스를 제공하기 위해 챙겨야 할 실용적인 보안 가이드.

## 목적
최근 P 사이트의 개인 정보 유출 사태에서 보듯이 보안은 하면 좋고 안해도 그만인 요소가 아니라 고객과 비즈니스를 보호하기 위해서는 우선적으로 챙겨야 할 핵심 요소입니다.
 
보안을 소홀히 하거나 관심이 없어서 해킹을 당하거나 정보 유출이 발생한다면 사용자 이탈, 평판 하락등 심각한 피해를 입을 수 있으며 특히 강화된 개인정보보호법과 정보통신망법에 의해 큰 사업상의 손실을 입을 수도 있습니다.
 
하지만 기밀 정보를 보호하고 시스템을 안전하게 유지하는 것은 많은 보안 지식을 필요로 하므로 경험이 많지 않다면 쉽지 않은 일입니다.

이 글에서는 리눅스를 기반으로 웹 서비스를 제공할 경우 필수적으로 챙겨야 할 보안의 핵심 사항을 정리해 보고 실무에서 활용할 수 있는 베스트 프랙티스를 제공하고자 합니다.

리눅스 배포판은 RHEL(Red Hat Enterprise Linux)과 이의 파생판인 CentOS와 우분투(Ubuntu) 를 대상으로 작성하였으며 웹 서버, 애플리케이션 서버, 인프라 서비스등은 오픈 소스 제품만을 다루고 있습니다.


## 독자
개발자와 운영자, 아키텍트등 서비스를 개발하고 운영하는 기술자들을 대상으로 합니다.


## Disclaimer
이 문서는 참고하기 위한 자료일뿐이며 여기에 있는 내용을 따라 했다고 하여 보안이 보장되지 않으며 잘못된 결과에 대해서는 저자는 아무 책임이 없습니다.

### 제안과 기여
본 문서에서 틀린 부분이나 수정/추가되야 할 부분이 있으면 Fork 후에 PR 을 날려주시기 바라며 제안은 issue 를 통해서 해주시면 됩니다.


### 목차 
* [운영체제](https://github.com/lesstif/security-best-practices/linux.md) - 보안을 위한 리눅스 설치와 관리
* [보안 시스템](https://github.com/lesstif/security-best-practices/firewall-selinux.md) - iptales/firewalld 방화벽과 SELinux 등 보안 시스템
* [웹 서버](https://github.com/lesstif/security-best-practices/web-server.md) - apache httpd/nginx 웹 서버
* [WAS](https://github.com/lesstif/security-best-practices/web-app-server.md) - tomcat, php fpm등 application server
* [데이타 보호](https://github.com/lesstif/security-best-practices/encryption.md) - 해시, 대칭키/공개키 기반 데이타 암복호화로 데이타 보호하기
* [시큐어 코딩](https://github.com/lesstif/security-best-practices/secure-coding.md) - SQL Injection, CSRF, XSS 등을 방지하기 위한 secure coding 가이드.

