# UrlOverlayManager

방송 중 사용하는 웹페이지와 오버레이를 한곳에서 관리하는 Windows용 도구입니다. 소스 코드는 비공개이며, 이 저장소에는 검증된 실행 파일과 SHA-256 체크섬만 공개합니다.

## 다운로드

- [최신 버전 다운로드](https://github.com/GStar0325/UrlOverlayManager-Releases/releases/latest)
- [Windows x64 실행 파일 바로 받기](https://github.com/GStar0325/UrlOverlayManager-Releases/releases/latest/download/UrlOverlayManager-win-x64.exe)

별도 설치 프로그램 없이 `UrlOverlayManager-win-x64.exe`를 실행하면 됩니다. .NET Runtime은 실행 파일에 포함되어 있습니다.

## 처음 실행할 때

- 프로그램은 개인 문서나 다운로드 폴더처럼 쓰기 가능한 위치에 두는 것을 권장합니다.
- WebView2 Runtime이 없는 PC에서는 Microsoft 공식 설치 페이지를 안내합니다.
- 상용 코드 서명이 적용되지 않아 Windows SmartScreen 경고가 표시될 수 있습니다. 반드시 이 저장소의 Releases에서 받은 파일인지 확인해 주세요.
- 이후 버전은 프로그램의 `업데이트 확인` 기능으로 설치할 수 있습니다.

## 서비스 연동

- Song Studio와 치지직 등 외부 서비스는 사용자 본인의 계정으로 로그인해야 합니다.
- Song Studio 노래책은 로그인된 사용자의 `/my/songbook` 페이지를 사용합니다.
- TJ노래방 앱이 실행되지 않은 상태에서는 관련 기능이 자동으로 비활성화되며, 다른 기능은 계속 사용할 수 있습니다.

## 데이터와 개인정보

설정과 로그인 데이터는 각 PC의 로컬 사용자 폴더에 저장되며 공개 실행 파일에 포함되지 않습니다. 배포 파일에는 개발자의 계정 정보나 개인 설정도 포함하지 않습니다.

## 파일 검증

각 릴리스에는 실행 파일과 함께 `UrlOverlayManager-win-x64.exe.sha256` 파일이 제공됩니다. PowerShell에서는 다음 명령으로 실행 파일의 SHA-256 값을 확인할 수 있습니다.

```powershell
Get-FileHash .\UrlOverlayManager-win-x64.exe -Algorithm SHA256
```