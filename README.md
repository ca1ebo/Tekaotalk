<p align="center"><img src="./app/assets/images/SealCircle.png" width="150px" height="150px" alt="aventium softworks"></p>

<h1 align="center">Tekaotalk Launcher</h1>

<em><h5 align="center">(formerly Electron Launcher)</h5></em>

[<p align="center"><img src="https://img.shields.io/github/actions/workflow/status/dscalzi/HeliosLauncher/build.yml?branch=master&style=for-the-badge" alt="gh actions">](https://github.com/dscalzi/HeliosLauncher/actions) [<img src="https://img.shields.io/github/downloads/dscalzi/HeliosLauncher/total.svg?style=for-the-badge" alt="downloads">](https://github.com/dscalzi/HeliosLauncher/releases) <img src="https://forthebadge.com/images/badges/winter-is-coming.svg"  height="28px" alt="winter-is-coming"></p>

<p align="center">Java, Forge 또는 기타 모드 설치에 대한 걱정 없이 모드 서버에 접속해 보세요. 모든 번거로운 과정은 런처에서 자동으로 처리해 드립니다.</p>

![Screenshot 1](https://i.imgur.com/6o7SmH6.png)
![Screenshot 2](https://i.imgur.com/x3B34n1.png)

### 주요 기능

* 🔒 계정 통합 관리
  - 여러 계정을 추가하고 간편하게 전환할 수 있습니다.
  - Microsoft (OAuth 2.0) 및 Mojang (Yggdrasil) 인증을 완벽하게 지원합니다.
  - 계정 정보는 별도로 저장되지 않으며 Mojang 서버로 직접 전송되어 안전합니다.
* 📂 효율적인 리소스 관리
  - 새로운 클라이언트 업데이트가 출시되면 즉시 적용할 수 있습니다.
  - 실행 전 파일의 무결성을 검증하며, 손상되었거나 잘못된 파일은 자동으로 다시 다운로드합니다.
* ☕ 자바(Java) 버전 자동 검증
  - 시스템에 호환되지 않는 버전의 자바가 설치되어 있다면, 적절한 버전을 자동으로 설치해 드립니다.
  - 사용자가 사전에 자바를 직접 설치할 필요가 없어 편리합니다.
* 📰 뉴스 피드 내장: 최신 소식을 런처 내부에서 바로 확인할 수 있습니다.
* ⚙️ 직관적인 설정 관리: 자바 제어판을 포함한 모든 설정을 손쉽게 관리할 수 있습니다.
* 자체 운영 서버 지원
  - 여러 서버 구성을 자유롭게 전환할 수 있습니다.
  - 선택한 서버의 현재 접속자 수를 실시간으로 확인할 수 있습니다.
* 자동 업데이트: 런처가 스스로 업데이트를 진행하여 항상 최신 상태를 유지합니다.
* 서비스 상태 확인: Mojang 서비스의 가동 여부를 실시간으로 모니터링합니다.

이 외에도 다양한 기능이 준비되어 있습니다. 런처를 설치하여 직접 확인해 보시기 바랍니다.

#### 도움이 필요하신가요? [위키(Wiki)를 참조하세요.][wiki]
#### 프로젝트가 마음에 드신다면 저장소에 Star를 남겨주세요!

## 다운로드

[GitHub Releases](https://github.com/dscalzi/HeliosLauncher/releases)에서 다운로드할 수 있습니다.

#### 최신 릴리스

[![](https://img.shields.io/github/release/dscalzi/HeliosLauncher.svg?style=flat-square)](https://github.com/dscalzi/HeliosLauncher/releases/latest)

#### 최신 프리 릴리스
[![](https://img.shields.io/github/release/dscalzi/HeliosLauncher/all.svg?style=flat-square)](https://github.com/dscalzi/HeliosLauncher/releases)

지원되는 플랫폼

[릴리스](https://github.com/dscalzi/HeliosLauncher/releases) 탭에서 다운로드하는 경우, 사용 중인 시스템에 맞는 설치 프로그램을 선택하세요.

| 플랫폼 | 파일 |
| -------- | ---- |
| Windows x64 | Helios-Launcher-setup-VERSION.exe |
| macOS x64 | Helios-Launcher-setup-VERSION-x64.dmg |
| macOS arm64 | Helios-Launcher-setup-VERSION-arm64.dmg |
| Linux x64 | Helios-Launcher-setup-VERSION.AppImage |

## 콘솔

콘솔을 열려면 다음 단축키를 사용하세요.

ctrl + shift + i

반드시 콘솔 탭이 선택되었는지 확인하시기 바랍니다. 코드의 동작 원리를 정확히 파악하지 못했다면 붙여넣기를 삼가 주세요. 잘못된 코드를 실행할 경우 보안상 위험이 발생할 수 있습니다.

#### 출력을 파일로 내보내기

콘솔 출력을 내보내려면 콘솔 아무 곳이나 마우스 오른쪽 버튼으로 클릭하고 Save as..를 클릭하세요.

![console example](https://i.imgur.com/T5e73jP.png)


## 개발

이 섹션은 기본적인 개발 환경 설정에 대해 설명합니다.

### 시작하기

시스템 요구 사항

* [Node.js][nodejs] v20

---

저장소 복제 및 의존성 설치

git clone https://github.com/dscalzi/HeliosLauncher.git
cd HeliosLauncher
npm install

---

애플리케이션 실행

npm start

---

설치 프로그램 빌드

현재 사용 중인 운영체제에 맞춰 빌드하려면 다음 명령어를 사용하세요.

npm run dist

특정 플랫폼용 빌드:

| 플랫폼 | 명령어 |
| ----------- | -------------------- |
| Windows x64 | npm run dist:win |
| macOS | npm run dist:mac |
| Linux x64 | npm run dist:linux |

macOS용 빌드는 Windows/Linux에서 작동하지 않을 수 있으며, 그 반대의 경우도 마찬가지입니다.

---

### Visual Studio Code

런처의 모든 개발은 [Visual Studio Code][vscode]를 사용하여 진행해야 합니다.

.vscode/launch.json에 다음 내용을 붙여넣으세요.

```JSON
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug Main Process",
      "type": "node",
      "request": "launch",
      "cwd": "${workspaceFolder}",
      "program": "${workspaceFolder}/node_modules/electron/cli.js",
      "args" : ["."],
      "outputCapture": "std"
    },
    {
      "name": "Debug Renderer Process",
      "type": "chrome",
      "request": "launch",
      "runtimeExecutable": "${workspaceFolder}/node_modules/.bin/electron",
      "windows": {
        "runtimeExecutable": "${workspaceFolder}/node_modules/.bin/electron.cmd"
      },
      "runtimeArgs": [
        "${workspaceFolder}/.",
        "--remote-debugging-port=9222"
      ],
      "webRoot": "${workspaceFolder}"
    }
  ]
}
```

이 설정은 두 가지 디버그 구성을 추가합니다.

#### Debug Main Process

Electron의 메인 프로세스를 디버깅할 수 있게 해줍니다. 개발자 도구 창을 열어 렌더러 프로세스의 스크립트를 디버깅할 수 있습니다.

#### Debug Renderer Process

Electron의 렌더러 프로세스를 디버깅할 수 있게 해줍니다. 이를 위해서는 Debugger for Chrome 확장 프로그램을 설치해야 합니다.

**이 디버그 구성에서는 개발자 도구 창을 동시에 열 수 없습니다. 중복 실행 시 프로그램이 종료될 수 있으니 유의하시기 바랍니다.**

---

### 제3자 사용 시 주의사항

본 프로그램은 무료 소프트웨어입니다. 타 플랫폼에서 활용하실 경우 원작자 정보를 명시하고 원본 소스 링크를 반드시 첨부해 주시기 바랍니다.

Microsoft 인증 설정에 대한 자세한 가이드는 다음 문서에서 확인하실 수 있습니다:
https://github.com/dscalzi/HeliosLauncher/blob/master/docs/MicrosoftAuth.md

---

## 리소스

* [Wiki][wiki]
* [Nebula (Create Distribution.json)][nebula]
* [v2 Rewrite Branch (Inactive)][v2branch]


---

### 게임에서 만나요.


[nodejs]: https://nodejs.org/en/ 'Node.js'
[vscode]: https://code.visualstudio.com/ 'Visual Studio Code'
[mainprocess]: https://electronjs.org/docs/tutorial/application-architecture#main-and-renderer-processes 'Main Process'
[rendererprocess]: https://electronjs.org/docs/tutorial/application-architecture#main-and-renderer-processes 'Renderer Process'
[chromedebugger]: https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome 'Debugger for Chrome'
[discord]: https://discord.gg/zNWUXdt 'Discord'
[wiki]: https://github.com/dscalzi/HeliosLauncher/wiki 'wiki'
[nebula]: https://github.com/dscalzi/Nebula 'dscalzi/Nebula'
[v2branch]: https://github.com/dscalzi/HeliosLauncher/tree/ts-refactor 'v2 branch'
