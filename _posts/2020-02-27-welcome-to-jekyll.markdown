---
layout: post
title:  "블로그 만들기"
date:   2020-02-27 13:25 +0530
categories: Javascript ReactJS Jekyll
---

<h2> 블로그 스펙 </h2>
Template : plainwhite  
Jekyll : 3.8.6  
자세한 내용은 여기 사이트로 <a> https://github.com/thelehhman/plainwhite-jekyll </a>


<h2> 블로그 개설하면서 겪은 트러블 이슈 </h2>
1. 윈도우에 Jekyll 설치가 힘들었음  
개인적으로 웹 개발 시에 Jetbrain을 주로 사용하는데, Window prompt with Ruby 에서 Jekyll을 아직 설치하지 못해서 Linux에 설치해서 작업함.  
 이 부분은 수정하면 다시 적을 예정  
 
2. _posts/ 에 post 된 글들을 저장하는데 파일 명에도 특정한 template이 있을 줄 생각도 못했음.  
처음에 rename 했다가 글이 갱신이 안 되어서 파일명을 되돌렸는데 (이 때, 파일명 되돌리는 것도 잘못 되돌렸다가 문제 해결하는데 시간 낭비함....)

3. .md 파일 작성하는 방법.  레포트 적을 때도 .md 파일은 평소에 작성하는 문서들이랑 포맷이 달라서 항상 헷갈렸다.  

4. 블로그 배포시에 발생한 에러.  
```
The tag seo on line 8 in _includes/head.html is not a recognized Liquid tag.
``` 
분명 로컬에서는 문제없이 돌아갔는데 에러가 생기더라  
기존  
``` _config.yml ```   
파일의
```
plugins_dir: 
  - jekyll-seo-tag 
``` 
에서 
```
gems:
- jekyll-seo-tag
plugins_dir:
 - jekyll-seo-tag 
```
로 변경해주었다.  
 다만 기존에 Gemfile 이라는 파일이 있는데 _config.yml에  gems를 추가해줘야 하는가에 대한 의문이 들었음.  
 나중에 시간 날 때 Gemfile과 _config를 찾아봐야할듯  (지금이 아침7시라 졸려서 다음 기회에 찾아봐야겠다.)

<h2> 블로그 더 발전시키려면? </h2>
1.  카테고리를 나누자

2.  ~~매번 date를 수동으로 계산해줘야 하는건가?   뭔가 더 쉽게 만드는 방법이 있지 않을까?~~  
~~=> 다른 사람들 gitblog 레포 가보니까 직접 입력하시는 듯 하다.~~
=> 무조건적으로 설정을 저렇게 해야함.  
https://jekyllrb.com/docs/posts/


3.  게시글을 볼 때 제목만 링크가 걸림.  
뭔가 블로그 본문을 눌렀을 때도 이동하는게 사용자 입장에서 좋을거 같다.  
다만 카테고리 누르면 카테고리에 맞는 글들만 이동해야할까? 아니면 home에서 누르면 해당 게시글로 가고 게시글에서 카테고리 누르면 카테고리 글들만 모아서 볼 수 있게 해야할까?  
이 부분을 정하면 template을 맞춰서 바꿔야겠다.  


<h2>블로그 명령어 </h2> 
```vim
jekyll serve  #로컬 테스팅
``` 
저장을 잘 하고 세팅은 나중에 더 바꿀듯하다.

Last Update : 2020-05-21
