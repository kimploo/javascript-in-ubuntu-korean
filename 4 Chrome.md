---
title: 'JS 개발 환경 세팅 (Chrome)'
metaTitle: '우분투로 자바스크립트 개발하기 - 4. Chrome'
metaDescription: '웹 개발의 기본, 크롬을 우분투에 설치해봅시다.'
---

2020년 3월 현재, 많은 웹사이트들이 크롬을 기준으로 만들어지고 있습니다. 또한, 자바스크립트를 공부하기에 적합한 개발자 콘솔을 제공합니다. 앞으로 배우실 React, Redux를 배우면서도 다른 브라우져가 아닌 크롬에서 활용할 수 있는 다양한 익스텐션들을 활용하기 위해서라도, **크롬은 꼭 설치하시는 것이 좋습니다**.

우분투에서 크롬을 깔아보겠습니다. 역시 CLI로 한번 깔아볼까요? 우선 크롬 설치 파일을 받아보겠습니다. 설치 파일을 저장하기 위해 `/home` 폴더 최 상단에 `apps`라는 폴더를 만들어보겠습니다. 무슨 말인지 잘 모르시겠다면 일단 한번 따라해볼까요?

터미널을 여시고 `cd ~` 을 입력한 뒤에 `mkdir apps` 라는 명령어로 `apps` 폴더를 만들어보겠습니다. 이후에 아시겠지만 `cd ~` 은 `/home` 폴더로 이동한 것이고, `mkdir apps` 는 그 곳에 `apps`라는 새로운 폴더를 만든 것입니다. 윈도우의 "새 폴더"와 같은 작업입니다. 이후에 `cd apps` 라는 명령어를 통해 폴더간 이동 (개발자들은 왠지 모르게 디렉토리라고 많이 합니다)을 한 후, 크롬 설치 파일을 받아봅시다. `wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb`

    cd ~
    mkdir apps
    cd apps
    wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

![4%20Chrome/_2020-03-12_21-27-02.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/4-chrome/_2020-03-12_21-27-02.png)

설치가 되었는지 확인해볼까요? 왼쪽 하단의 프로그램 표시 버튼을 누르고, `chrome` 으로 검색해보시면 아마 크롬을 찾으실 수 있을겁니다.

![4%20Chrome/_2020-03-12_21-26-27.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/4-chrome/_2020-03-12_21-26-27.png)

클릭해볼까요? 잘 실행되는 모습입니다 :)

![4%20Chrome/_2020-03-12_21-28-39.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/4-chrome/_2020-03-12_21-28-39.png)
