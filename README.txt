구구단 놀이터 Android APK 자동 빌드 프로젝트

[Android Studio 없이 APK 만들기 - GitHub Actions 이용]
1. https://github.com 에 로그인 후 New repository를 눌러 새 저장소를 만듭니다.
   이름 예: GugudanAndroid / Public 또는 Private 선택 / Create repository
2. 이 ZIP 압축을 풀고 GugudanAndroid 폴더 안의 파일과 폴더 전체를 GitHub 저장소에 업로드합니다.
   (웹에서 Add file > Upload files로 업로드하거나 GitHub Desktop을 사용해도 됩니다.)
3. 저장소의 Actions 탭으로 이동합니다.
4. 'Build Gugudan APK' workflow가 보이면 선택하고 'Run workflow'를 누릅니다.
   처음 업로드/커밋 시 자동 실행되기도 합니다.
5. 실행이 완료되면 녹색 체크 표시의 실행 항목을 열고 아래 Artifacts에서
   gugudan-debug-apk 를 다운로드합니다.
6. ZIP artifact를 풀면 app-debug.apk 파일이 있습니다. Android 휴대폰으로 보내 설치합니다.
   설치 시 안내가 나오면 해당 앱/브라우저에 '알 수 없는 앱 설치' 권한을 허용하세요.

[프로젝트에서 제공하는 앱]
- 2~9단 선택 및 전체 단 랜덤 퀴즈
- 구구단 연습 보기
- 10문제 퀴즈, 점수/연속정답 보너스, 최고 점수 저장
- 인터넷 없이 실행 (외부 웹폰트 링크 제거)

[Android Studio로 직접 빌드]
프로젝트 폴더를 Android Studio에서 Open 후 Gradle Sync를 기다리고,
Build > Build Bundle(s) / APK(s) > Build APK(s)를 선택합니다.
