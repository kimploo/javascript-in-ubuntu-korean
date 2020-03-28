---
title: '자바스크립트 개발 in 우분투, FAQ'
metaTitle: '자바스크립트 개발 in 우분투, FAQ'
metaDescription: '자바스크립트로 우분투롤 개발할 때 가장 먼저 질문하게 되는 점을 정리합니다.'
---

# 이제 여러분은 자바스크립트 개발을 우분투에서 하기 위한 준비가 충분히 되었습니다!

실제로 개발을 진행하면서 이런저런 세팅을 만져보면서 직접 우분투와 가까워지는 시간을 가져보는 것을 추천 드립니다. 사실 앞으로도 하셔야 할 세팅들이 아주 많습니다. 맥을 사용하시던 분은 단축키가 반대인 것을 바꾸고 싶을 것이고, 윈도우를 사용하시던 분은 한영키가 작동이 잘 되지 않는 등 다양한 문제가 있습니다. 아래 링크들은 제가 우분투를 사용하면서 도움이 많이 됬던 레퍼런스입니다. 자신의 문제가 아래 레퍼런스와 관련이 되어 있다면, 들어가보고 실제로 실습을 해보시기 바랍니다.

## Your best ubuntu FAQ

[Highest Voted Questions](https://askubuntu.com/questions?tab=Votes)

## How to install package

[AptGet/Howto](https://help.ubuntu.com/community/AptGet/Howto)

## How to uninstall package

[How can I uninstall software?](https://askubuntu.com/questions/1143/how-can-i-uninstall-software)

## 우분투 기본 레포 미러를 카카오로 설정

⇒ `sudo apt update` 가 도대체 언제 끝나는지 모르겠다면..

[[Ubuntu] 기본 repo mirror를 kakao mirror로 바꾸기](https://seonift.github.io/2019/06/21/Ubuntu-%EA%B8%B0%EB%B3%B8-repo-mirror%EB%A5%BC-kakao-mirror%EB%A1%9C-%EB%B0%94%EA%BE%B8%EA%B8%B0/)

위 안내대로 하고 나서 혹시 `sudo apt update`에 문제가 생겼다면, 아래 글을 읽고 직접 `/etc/apt/source/list` 파일을 수정해야 합니다.

[What is the correct output of cat /etc/apt/sources.list?](https://askubuntu.com/questions/443036/what-is-the-correct-output-of-cat-etc-apt-sources-list/443075#443075)

## install slack

[install Slack](https://linuxize.com/post/how-to-install-slack-on-ubuntu-18-04/)

## install lotion (unofficial notion app)

[puneetsl/lotion](https://github.com/puneetsl/lotion)

## 우분투는 카톡 안되나요?

[카카오톡 우분투에서 쓰기](6%20FAQ/Untitled.md)

## use macOS Key bindings / 키 매핑을 바꾸고 싶어요

[How to make keyboard work like OSX System Wide?](https://askubuntu.com/a/808588)

## install zoom in ubuntu

[Installing Zoom on Linux](https://support.zoom.us/hc/en-us/articles/204206269-Installing-Zoom-on-Linux)

## how to install yarn in ubuntu

[Yarn](https://classic.yarnpkg.com/en/docs/install/#debian-stable)

## 와이파이가 안되요!

`sudo apt install linux-generic-hwe-18.04` 을 해보세요. 노트북이 최신 기종이라서 생기는 문제일 수 있습니다. 이 명령어를 실행한 후에도 해결이 되지 않는다면, 직접 무선 랜카드의 제품 명을 확인하고 그에 해당하는 드라이버를 설치하셔야 됩니다. 우선은 직접 랜선을 연결하셔서 쓰셔야겠네요.

[WiFi Adapter AX201 Not Found: Ubuntu 18.04](https://askubuntu.com/questions/1196308/wifi-adapter-ax201-not-found-ubuntu-18-04)

## 파이어폭스에서 동영상 플레이가 안되요

[Playing Videos in Firefox](https://askubuntu.com/questions/1035661/playing-videos-in-firefox)

## 컴퓨터 부품들이 잘 작동하는지 보고싶어요

`sudo apt-get install hardinfo`

[How can I find my hardware details?](https://askubuntu.com/questions/31618/how-can-i-find-my-hardware-details)

## vim이 뭔가요? 써보고 싶어요

[How to install full version of Vim on Ubuntu](https://www.simplified.guide/ubuntu/install-vim)

## vim에서 한글 입력도 안되고 너무 불편해요

[VIM 을 IDE 처럼 사용하기(Plugin 설정)](https://medium.com/@jjeaby/vim-%EC%9D%84-ide-%EC%B2%98%EB%9F%BC-%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0-plugin-%EC%84%A4%EC%A0%95-87b40c5bfc14)

## zsh, oh-my-zsh가 뭔가요?

[ohmyzsh/ohmyzsh](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH)

## mysql을 다시 설치하고 싶어요.

    sudo apt-get remove --purge mysql-server mysql-client mysql-common
    sudo apt-get remove --purge mysql-client-core-5.5
    sudo apt-get autoremove
    sudo apt-get autoclean
    sudo rm -rf /var/lib/mysql
    sudo apt-get install mysql-server
    sudo apt-get install mysql-client

[](https://github.com/codestates/help-desk/issues/1179#issuecomment-583950154)
