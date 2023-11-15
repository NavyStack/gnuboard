# gnuboard
[![Check for updates](https://github.com/NavyStack/gnuboard/actions/workflows/check-update.yml/badge.svg)](https://github.com/NavyStack/gnuboard/actions/workflows/check-update.yml)
<br>
[![Docker Image CI](https://github.com/NavyStack/gnuboard/actions/workflows/docker-image.yml/badge.svg)](https://github.com/NavyStack/gnuboard/actions/workflows/docker-image.yml)

[깃허브 바로가기](https://github.com/NavyStack/gnuboard)
<br>
[도커허브 바로가기](https://hub.docker.com/r/navystack/gnuboard)

- [x] 설명 추가하기
- [x] 도커 이미지 빌드


---

## Traefik을 사용하는 것을 가정하고 제작되었습니다.
* 인증서 관련 어려움을 해소할 수 있음.
* docker image를 사용한다는 것은, 코어를 수정하지 않고 Theme만 수정해서 사용한다는 것을 의미함.
* 초기 install 과정에서 `localhost`로 하드코딩 되어있는 부분을 회피할 수 있음.

## Traefik을 사용하지 않는다면

* Traefik을 사용하지 않는다면 해당 과정에서 어려움이 있다면 <br> `http://localhost/install` 부분을 포트 지정해서 예를 들어 `http://localhost:9876/install`과 같이 우회할 수있음.
* 그러나 인증서 관련해서는 직접 사용자가 설정해야합니다. 또는 리버스 프록시로 중계해야함. (본 이미지는  php, nginx 도커 공식이미지 이미지를 사용합니다. 방법은 유사합니다.)

Traefik에 대한 설정은 https://github.com/NavyStack/traefik/ 여기에서 참고하실 수 있습니다.
해당 레포에서 선행하신 후에 `docker compose up -d`하시면 됩니다.

모든 과정에서 어려움을 겪고 있다면, 주저하지 말고 github이슈나 [블로그](https://navystack.com/)의 아무 글에서 댓글을 작성해주세요. <br>
블로그는 로그인이 필요하지 않습니다.

---

모든 빌드 인수 및 관련된 파일은 https://github.com/NavyStack/gnuboard에서 확인하실 수 있습니다. 

---

모든 Docker 이미지와 마찬가지로, 여기에는 다른 라이선스(예: 기본 배포판의 Bash 등 및 포함된 기본 소프트웨어의 직간접적인 종속성)가 적용되는 다른 소프트웨어도 포함될 수 있습니다.

사전 빌드된 이미지 사용과 관련하여, 이 이미지를 사용할 때 이미지에 포함된 모든 소프트웨어에 대한 관련 라이선스를 준수하는지 확인하는 것은 이미지 사용자의 책임입니다.

기타 모든 상표는 각 소유주의 재산이며, 달리 명시된 경우를 제외하고 본문에서 언급한 모든 상표 소유자 또는 기타 업체와의 제휴관계, 홍보 또는 연관관계를 주장하지 않습니다.

---
