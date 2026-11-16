# 졸업시험대비 - Android 프로젝트

375문항 HTML 학습 앱을 Android WebView 컨테이너에 넣은 프로젝트입니다. 학습 데이터와 화면은 `app/src/main/assets/index.html`에 포함되어 인터넷 연결 없이 실행되도록 구성했습니다.

## Android Studio에서 APK 만들기
1. Android Studio에서 이 폴더를 엽니다.
2. SDK Platform 35 설치를 허용합니다.
3. 메뉴에서 **Build > Build Bundle(s) / APK(s) > Build APK(s)** 를 선택합니다.
4. 생성 파일: `app/build/outputs/apk/debug/app-debug.apk`

## GitHub Actions에서 빌드하기
프로젝트를 GitHub 저장소에 올린 뒤 Actions 탭에서 **Build shareable APK**를 실행합니다. 완료된 workflow의 Artifacts에서 `socialworker-level1-apk`를 내려받을 수 있습니다.

## 공유 및 설치
생성된 `app-debug.apk`를 다른 사람에게 전달하면 됩니다. 설치하는 사람은 Android 설정에서 해당 파일을 받은 앱(예: Chrome 또는 내 파일)에 대해 '알 수 없는 앱 설치 허용'을 켜야 할 수 있습니다. APK는 Android 기기용이며 iPhone에는 설치할 수 없습니다.

## 주의
- 이 프로젝트는 첫 공유용 debug APK를 빌드합니다. Google Play 등록용 서명/정책 설정은 별도입니다.
- 앱 내 진도/기록은 각 기기의 앱 저장공간에 저장되며 사용자 간 자동 동기화되지 않습니다.
- 공식 정답표가 제공되지 않아 정답 채점 기능은 임의로 추가하지 않았습니다.
