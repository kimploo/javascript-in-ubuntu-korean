---
title: 'JS 개발 환경 세팅 (VS Code)'
metaTitle: '우분투로 자바스크립트 개발하기 - Code Editor VS Code 설치'
metaDescription: '입문하기 가장 좋은 Code Editor VS Code를 설치하는 법에 대해서 배웁니다.'
---

이제 여러분은 자바스크립트 개발을 할 준비가 거의 되었습니다. 이제 코드 작성하러 가셔야죠! 코드는 정말로, 윈도우의 메모장 같은 곳에다가 적어서 작성하실 수도 있습니다! 하지만 2020년에는 뭔가 좀 더 효율적인 도구를 써보도록 할까요? 제가 추천하는 코드 에디터는 **Visual Studio Code** 입니다. 처음 개발을 하는 사람이 쓰기에 편리한 기능이 다수 내장되어 있습니다. 거의 IDE라고 불러도 될 만큼의 강력한 기능을 가지고 있습니다!

한번 설치해볼까요? 공식 홈페이지로 이동해보겠습니다.

[Visual Studio Code - Code Editing. Redefined](https://code.visualstudio.com/)

![5%20Visual%20Studio%20Code/_2020-03-12_21-07-54.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/5-vscde/_2020-03-12_21-07-54.png)

왼쪽에 우분투에서의 설치를 위한 `.deb` 파일을 다운로드 받습니다. 다운로드 받은 폴더로 한번 가볼까요? 저는 크롬을 설치했던 `apps` 폴더에 다운로드 받았습니다.

![5%20Visual%20Studio%20Code/_2020-03-12_21-32-12.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/5-vscde/_2020-03-12_21-32-12.png)

한번 터미널에서도 파일을 확인해볼까요? `ls -al` 이라는 명령어로, 현재 터미널이 위치해있는 디렉토리의 모든 파일 및 폴더 정보를 확인할 수 있습니다. 나중에 `.git` 같은 `.` 으로 시작하는 숨겨진 파일이나 폴더도 확인하실 수 있습니다. 이렇게 숨겨진 파일을 볼 수 있다는 것은 실제 세팅 파일이 어디에 있고 무엇을 고쳐야 하는지 이해할 수 있는 단초가 됨으로, 중요합니다!

![5%20Visual%20Studio%20Code/_2020-03-12_21-32-51.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/5-vscde/_2020-03-12_21-32-51.png)

아까 받았던 파일이 있는 것을 확인할 수 있습니다. 이 곳에서 아까 크롬을 설치했던 것 과 같은 명령어를 실행하셔야 됩니다. `sudo apt install ./code_1.43.0-1583783132_amd62.deb`

![5%20Visual%20Studio%20Code/_2020-03-12_21-34-05.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/5-vscde/_2020-03-12_21-34-05.png)

    sudo apt install ./code_1.43.0-1583783132_amd62.deb

막간을 이용해 내가 무슨 명령을 내린건지 한번 곱씹어볼까요? `apt`는 설명 드렸지만 일종의 패키지 설치 도구입니다. 이 패키지 설치 도구가 무언가를 루트 폴더에 설치를 하려면 `sudo` 권한이 필요합니다. 그래서 `sudo apt install` 이라는 설치 명령을 내렸는데요, 이번에는 `.deb` 패키지를 지정해줬습니다. 위치를 잘 명시해주었죠? `./code_1.43.0-1583783132_amd62.deb` 앞으로도 대부분의 `.deb` 패키지들을 다운을 받으시게 된다면, 이렇게 `apt`를 통해서 설치하실 수 있어야 합니다.

이제 여러분은 Visual Studio Code를 사용하실 수 있습니다. 크롬과 같은 방식으로 찾아서 실행시켜보세요!

![5%20Visual%20Studio%20Code/_2020-03-12_21-35-25.png](https://hongshik-blog-bucket.s3.ap-northeast-2.amazonaws.com/photos/ubuntu-starter/5-vscde/_2020-03-12_21-35-25.png)
