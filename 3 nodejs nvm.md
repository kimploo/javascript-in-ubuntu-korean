---
title: 'JS 개발 환경 세팅 (nodejs, nvm)'
metaTitle: '우분투로 자바스크립트 개발하기 - 3. nodejs, nvm 설치하기'
metaDescription: '자바스크립트 오픈소스 npm package를 활용하기 위한 nodejs, nvm 설치하는 방법입니다.'
---

우분투에서 자바스크립트 개발을 위한 환경을 세팅해보도록 하겠습니다. 여러분은 앞으로 `apt` 라는 강력한 CLI 툴을 사용하게 될 것입니다. apt는 (Advanced Packageing Tool) 이라는 뜻으로, 여러가지 패키지를 쉽게 설치할 수 있습니다. 특수한 패키지를 제외하고는 대부분 `apt`를 통해 설치할 수 있습니다. 아래 링크에서 사용법에 대해 자세히 설명이 되어있으니 한번 읽어보면 좋습니다!

[Apt](https://help.ubuntu.com/lts/serverguide/apt.html)

우선 앞으로 자바스크립트 개발을 위해서 꼭 설치해야 하는 `nodejs` 를 설치하겠습니다. 원래 자바스크립트는 웹 브라우져에서 웹 페이지를 동적으로 변화시키기 위해서 사용하던 단순 스크립트 언어였습니다. 하지만 웹 개발이 발전하면서 자바스크립트도 함께 급격히 발전했고, 이제는 `nodejs`를 통해서 여러분의 데스크톱 컴퓨터나, 서버에서도 작동시킬 수 있게 되었습니다. 이렇게 `nodejs`를 컴퓨터에 설치하시면, 브라우져에 웹 페이지를 띄우는 것 말고도 다양한 작업을 할 수 있게 됩니다. Full-Stack Development가 자바스크립트로 가능해진 주요한 이유입니다.

이 `nodejs`를 가장 효율적으로 사용할 수 있는 도구가 `nvm` 입니다. 뭐하는 녀석인지 궁금하다면 [한번 구글링을 해보시죠 :)](https://stackoverflow.com/questions/32660993/difference-between-npm-and-nvm) `nvm` 부터 설치 해볼까요? `nvm` 의 모든 소스코드를 보관하고 있는 깃허브로 이동합니다.

[nvm-sh/nvm](https://github.com/nvm-sh/nvm#install--update-script)

이동하셨나요? github 페이지를 자세히 읽어보시면 영어지만 어떤것을 하면 이 패키지를 사용할 수 있는지 잘 설명되어 있습니다. 하나씩 해보겠습니다.

![3%20nodejs%20nvm/_2020-03-12_20-34-18.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-34-18.png)

    curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash

음.. 왜 안되죠? 저는 이런 화면을 보고 있습니다.

![3%20nodejs%20nvm/_2020-03-12_20-35-35.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-35-35.png)

뭔 소린지는 잘 모르겠지만, 뭔가 추가로 설치를 해야 되는 것 같습니다. 사실 위 명령을 실행하기 위해서는 이 cURL이라는 패키지를 설치를 하셔야 합니다! 이런 메세지가 나왔다는 것은, 설치가 되어있지 않다는 의미입니다. 다음 기회에 꼭 설치해보세요. :D

그러면 다음에 적혀있는 명령어를 한번 쳐볼까요?

    wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash

![3%20nodejs%20nvm/_2020-03-12_20-37-02.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-37-02.png)

갑자기 무언가 되버리고 말았습니다. 뭔가 된 것 같죠? 터미널을 잘 읽어보시면 "터미널을 껏다가 키고 nvm을 사용해보세요"라고 적혀있습니다. 영어를 아무래도 잘 해야만 할 것 같지 않나요?

이제 아래의 커멘드를 입력해보세요

    nvm --version

이 커멘드는 `nvm`의 버젼을 확인하는 명령어지만, 설치가 잘 되었는지 확인할 수도 있는 커멘드이기도 합니다. 만약 어떤 프로그램을 깔았다면 이렇게 버젼 확인 커맨드가 무엇인지 확인해보세요. 그렇다면 설치가 잘 되었는지 확인하실 수 있습니다. 영어가 자신 있으시다면 `nvm --help` 로도 대부분의 명령어를 확인하실 수 있습니다.

이제 `nodejs`를 `nvm`을 통해서 설치하겠습니다. `nvm ls-remote --lts` 라는 명령어를 적으면 이런 화면을 보실 수 있습니다. `nvm` 뒤에 뭔가를 붙임으로써, 다른 동작을 할 수 있다는 점을 유념하셔야 합니다.

![3%20nodejs%20nvm/_2020-03-12_20-46-32.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-46-32.png)

겁나 많네요!

LTS라는 말 어디서 보지 않았나요? 우분투 설치할 때 LTS라는 말을 많이 보셨을 겁니다. LTS는 **Long Term Support**라는 말의 약자로, 이 버젼의 패키지를 오랫동안 지원하겠다는 의미입니다. 어떤 패키지든 LTS를 깔아야겠다 라는 느낌이 팍팍 오신다면, 센스가 좋으신겁니다!

그럼 2020년 3월 기준 최신 LTS 버젼을 설치하겠습니다. 가장 마지막에 최근 LTS라고 나와있는 12.16.1 버젼을 설치해볼까요? `nvm install 12.16.1` 라는 명령어로 설치할 수 있습니다.

![3%20nodejs%20nvm/_2020-03-12_20-53-18.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-53-18.png)

와우! `nodejs`를 설치하셨습니다! `nvm`은 다른 버젼의 `nodejs`도 사용할 수 있다는 것이 장점이기 때문에, 한번 10.13.0 버젼도 설치하고, 사용해보겠습니다! `nvm install 10.13.0`

![3%20nodejs%20nvm/_2020-03-12_20-56-42.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-56-42.png)

잘 하셨습니다! 이제 두가지 `nodejs` 버젼을 사용할 수 있습니다. 어떻게 버젼을 바꿔가면서 사용할 수 있을까요? 아래의 스크린샷을 참고해주세요. 더 다양한 기능이 있지만, 이 후 부터는 직접 공부하셨으면 좋겠네요!

![3%20nodejs%20nvm/_2020-03-12_20-58-07.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/3-nodejs-nvm/_2020-03-12_20-58-07.png)
