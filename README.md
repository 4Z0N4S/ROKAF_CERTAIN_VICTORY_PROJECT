# Ubuntu 14.04.5 LTS

### 01. Configuration
Goorm.io 컨테이너 시작 설정

    # DBus System daemon
    mkdir -p /var/run/dbus
    rm /var/run/dbus/*
    dbus-daemon --system

    # SSH Daemon
    /usr/sbin/sshd-original -D
    
### 02. Install
환경 설치

    ./01_ENVIRONMENT
    ./02_KAKAO
    
### 03. Applications
- `fcitx`, `fcitx-hangul`: 한글 키보드 입력용
- `tigervncserver` : VNC 서버 지원용 (기존 `tightvncserver`보다 지원성이 높음)
- `noVNC` : Websocketify를 이용한 웹 브라우저에서 접근할 수 있는 VNC 클라이언트(제공자 서버)
- `GNOME` : Desktop Environment

#### Development Applications
- `VSCode` : Visual Studio Code는 각종 Code에 대한 Editing을 수행할 수 있다.
- `Eclipse Oxygen` : Java 개발용 IDE.
- `PyCharm Community Edition` : Python 개발용 IDE.
