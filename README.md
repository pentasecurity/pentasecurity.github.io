## Penta Security Technical Blog
Penta Security 의 기술 블로그를 사용하기 위한 방법을 기술한 문서입니다.

블로그의 글을 작성하거나, 내용을 수정하기 전에 아래 두가지 문서에 대해서 숙지하고 작업을 해주세요.

* [GitHub Pages](https://pages.github.com/)
* [Jekyll](https://jekyllrb.com/)


## 글 작성 방법
* <code>_posts</code> 디렉토리에 다음과 같은 형식으로 글을 작성합니다.
1. 파일 이름 형식 : "yyyy-mm-dd-subject"
2. 상단 형식
```
---
layout: post
title: 펜타시큐리티 기술 블로그
description: 펜타시큐리티의 기술 블로그를 소개합니다.
author: kssim
tags: 공지
---
```
3. 본문은 markdown 형태로 작성합니다.
* 이미지 파일은 <code>assets/img/posts</code> 에 두고, 링크를 추가합니다.
* 기타 다른 파일은 <code>assets/files</code> 에 두고, 링크를 추가합니다.


## 글 작성자 정보 추가 방법
* <code>_authors</code> 디렉토리에 다음과 같은 형식으로 작성자 정보를 합니다.
1. 파일 이름 형식 : "작성자ID.md"
2. 상단 형식
```
---
layout: author
name: kssim
title: 심경섭
desc: Infrastrucutre Developer
image: assets/img/authors/kssim.jpg
background: assets/img/authors/kssim-background.jpg
link: https://github.com/kssim
---
```
* image 는 글 작성자 정보에 표시될 사진입니다.  
    * 사진 파일은 예제에 표시된 경로에 둡니다. <code>assets/img/authors/</code>
* background 는 글 작성자 정보 화면의 메인 사진입니다.
* link 는 글 작성자 이름을 클릭했을때 링크될 페이지입니다.


## 작성 글 테스트 방법
1. ruby-dev, gem bundler, build-essential 을 설치합니다.  
   * Debian 기준 <code>apt-get install ruby-dev gem bundler build-essential</code>  
2. Jekyll 3.6.2 버전 이상을 설치합니다.  
   * <code>gem install jekyll</code>  
   * liquid 패키지에서 문제가 생길수도 있는데, 시스템에 설치된 패키지를 삭제하고, 최신 버전을 받아주면 됩니다.
       * <code>gem install jekyll</code>
3. 소스 코드를 clone 받습니다.
4. 소스 코드의 최상단에서 <code>sudo bundle install</code>를 실행합니다.
5. jekyll 을 이용해서 서버를 띄웁니다.  
    * <code>jekyll serve -H [HOST IP] -P [PORT]</code>




## License
[Apache2 License](https://github.com/pentasecurity/pentasecurity.github.io/blob/master/README.md)
