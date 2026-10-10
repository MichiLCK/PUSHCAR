# 푸쉬카 리모컨 (PWA)

BMW 푸쉬카 대시보드(ESP32)를 안드로이드 크롬에서 블루투스로 조작하는 설치형 웹앱입니다.

## 파일
- index.html : 앱 화면과 블루투스 처리
- manifest.webmanifest : 앱 이름, 아이콘 (홈 화면 설치용)
- sw.js : 오프라인에서도 열리게 하는 서비스 워커
- icon-192.png, icon-512.png : 앱 아이콘

## GitHub Pages 에 올리기
1. github.com 에서 새 저장소 만들기 (예: pushcar), Public 선택
2. Add file > Upload files 로 이 폴더의 파일 5개를 모두 올리고 Commit
3. Settings > Pages > Branch 를 main, 폴더를 / (root) 로 선택 후 Save
4. 1~2분 뒤 https://아이디.github.io/pushcar/ 주소가 생김

## 폰에 설치
1. 안드로이드 크롬으로 위 주소 열기
2. 오른쪽 위 메뉴 > 앱 설치 (또는 홈 화면에 추가)
3. 홈 화면의 "푸쉬카" 아이콘으로 실행

## 펌웨어와 맞춰야 하는 값
index.html 위쪽의 SVC, CMD, STAT, CFG UUID 는 dash_test.ino 의 값과 같아야 합니다.
