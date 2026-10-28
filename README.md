# 이니쌤 VOCA

모바일 설치와 오프라인 화면 캐싱을 지원하는 단어 학습 PWA입니다.

## 설정 및 실행

1. `config.js`의 `appUrl`을 배포된 Google Apps Script 웹 앱 주소(`https://script.google.com/macros/s/.../exec`)로 설정합니다. 비워 두면 예시 단어를 사용하는 체험 모드로 실행됩니다.
2. 저장소의 루트 디렉터리를 정적 웹 호스팅에 배포합니다. 서비스 워커와 PWA 설치 기능은 HTTPS 또는 로컬 개발 환경에서 제공되어야 합니다.
3. 사이트를 열고 브라우저의 설치 기능을 사용해 앱으로 추가합니다. 서비스 워커가 앱 파일과 아이콘을 캐시하므로 화면은 오프라인에서도 열 수 있습니다.

앱 진입 파일은 `index.html`이며, 설치 메타데이터는 `manifest.webmanifest`, 캐싱 동작은 `sw.js`, 앱 설정은 `config.js`에서 관리합니다. PWA 아이콘은 `icons/`에 있습니다.
