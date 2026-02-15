<p align="center"><img src="./app/assets/images/SealCircle.png" width="150px" height="150px" alt="aventium softworks"></p>

<h1 align="center">Tekaotalk Launcher</h1>

<em><h5 align="center">(formerly Electron Launcher)</h5></em>

[<p align="center"><img src="https://img.shields.io/github/actions/workflow/status/dscalzi/HeliosLauncher/build.yml?branch=master&style=for-the-badge" alt="gh actions">](https://github.com/dscalzi/HeliosLauncher/actions) [<img src="https://img.shields.io/github/downloads/dscalzi/HeliosLauncher/total.svg?style=for-the-badge" alt="downloads">](https://github.com/dscalzi/HeliosLauncher/releases) <img src="https://forthebadge.com/images/badges/winter-is-coming.svg"  height="28px" alt="winter-is-coming"></p>

<p align="center">Java, Forge 또는 기타 모드 설치에 대해 걱정할 필요 없이 모드 서버에 접속하세요. 모든 번거로운 과정은 저희가 대신 처리해 드립니다.</p>

![Screenshot 1](https://i.imgur.com/6o7SmH6.png)
![Screenshot 2](https://i.imgur.com/x3B34n1.png)

## Features

* 🔒 전체 계정 관리.
  * 여러 계정을 추가하고 쉽게 전환할 수 있습니다.
  * Microsoft (OAuth 2.0) 및 Mojang (Yggdrasil) 인증을 완벽하게 지원합니다.
  * 계정 정보는 저장되지 않으며 Mojang으로 직접 전송됩니다.
* 📂 효율적인 에셋 관리.
  * 새로운 클라이언트 업데이트가 출시되면 바로 받을 수 있습니다.
  * 파일은 실행 전에 검증되며, 손상되거나 잘못된 파일은 다시 다운로드됩니다.
* ☕ 자동 Java 검증.
  * 호환되지 않는 버전의 Java가 설치되어 있을 경우, 올바른 버전을 자동으로 설치해 드립니다.
  * 런처를 실행하기 위해 Java를 미리 설치할 필요가 없습니다.
* 📰 런처에 기본 내장된 뉴스 피드.
* ⚙️ Java 제어판을 포함한 직관적인 설정 관리.
* 모든 자체 서버 지원.
  * 서버 구성을 간편하게 전환할 수 있습니다.
  * 선택한 서버의 플레이어 수를 확인할 수 있습니다.
* 자동 업데이트. 맞습니다, 런처가 스스로 업데이트를 진행합니다.
* Mojang 서비스의 상태를 확인하세요.

이것이 전체 목록은 아닙니다. 런처를 다운로드하고 설치하여 모든 기능을 직접 확인해 보세요!

#### 도움이 필요하신가요? [위키를 확인하세요.][wiki]

#### 프로젝트가 마음에 드시나요? 저장소에 Star를 남겨주세요!

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

콘솔 탭이 선택되어 있는지 확인하세요. 무엇을 하는 코드인지 100% 확신하지 못한다면 콘솔에 아무것도 붙여넣지 마십시오. 잘못된 내용을 붙여넣으면 민감한 정보가 노출될 수 있습니다.

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

현재 사용 중인 플랫폼용으로 빌드하려면:

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

이 디버그 구성을 사용하는 동안에는 개발자 도구 창을 열 수 없다는 점에 유의하세요. Chromium은 하나의 디버거만 허용하므로, 다른 디버거를 열면 프로그램이 충돌합니다.

---

### 제3자 사용 시 주의사항

원작자에게 크레딧을 제공하고 원본 소스 링크를 남겨주세요. 이것은 무료 소프트웨어이므로 최소한 이 정도는 지켜주시기 바랍니다.

Microsoft 인증 설정에 대한 지침은 https://github.com/dscalzi/HeliosLauncher/blob/master/docs/MicrosoftAuth.md 를 참조하세요.

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
