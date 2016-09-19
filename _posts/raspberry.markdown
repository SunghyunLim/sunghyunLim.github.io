# 라즈베리파이 개발환경 만들기
## 초기 구성
- SD 카드 포멧
  - 라즈베리파이용 마이크로 SD 포멧하는 툴(SDForamtter)
  - URL : https://www.sdcard.org/downloads/formatter_4/eula_mac/
  - 아래쪽에 Accept 해서 내려받은 뒤 설치
  - RASPBERRY이름으로 새로 포멧함
- 라즈베리 이미지 내려받기
  - URL : https://www.raspberrypi.org/downloads/
  - 압축 풀어서 SD 카드에 올려놓기
  - NOOBS 이미지 다운로드. 동영상 : https://vimeo.com/90518800 참조
  - 압축 풀고 SD카드에 밀어넣기

## 설치
- 키보드+마우스+무선랜 꼽고 SD카드 삽입. 전원 넣으면 바로 시작
  - 주의: 핀에 금속이 닿으면 소트 나면서 재부팅됨

## 한글 구성
- sudo apt-get update (라이브러리 업데이트)
- sudo apt-get install ibus (다국어 입력기)
- sudo apt-get install ibus-hangul (ibus 한글 입력 패키지)
- sudo apt-get install ttf-unfonts-core (라즈베리파이 한글 기본 폰트)

## 한글 Locale 적용
- [Menu] -> [기본설정] -> [Raspberry Pi Configuration]
- Localisation 텝 클릭 -> Set Locale... 클릭
- Language : ko , Country : KR , Charcter Set : UTF-8 선택

## Timezone
- Asia / Seoul 타임존 설정
- 저장할 때 _재부팅_

## iBus, Font
- iBus 환경설정 -> 입력방식 -> 추가 -> 한국어 추가 
- sudo apt-get install fonts-nanum-coding

## 아두이노
- 아두이노 설치 : sudo apt-get install arduino

## 참고
- http://blog.naver.com/otlzero/220796907324
