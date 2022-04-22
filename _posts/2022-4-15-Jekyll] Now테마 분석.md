---
layout: single
title : "Jekyll] Jekyll-now 테마 구조 분석"
categories : [Jekyll]
---

0. Jekyll 한글가이드 문서 링크  
    https://jekyllrb-ko.github.io/

1. 골격(Root 아래 5개 카테고리 구성)  
     / (root)  
        >> _includes  
        >> _layouts  
        >> _posts  
        >> _sass  
        >> images  

2. 세부항목  
    1> _includes  
    2> _layouts  
        > default.html  
            >> 상단 메뉴바 기본 Template HTML  
            * baseurl, url 등의 값은 site.'사용할 객체명'을 통해 _config.yml에서 가져온다.
    3> _posts  
    4> _sass  
    5> _images  


* site.data.[파일명]
  > _data 폴더내 파일을가져온다. Now 기본 테마에는 없다.

* Liquid Tag를 

3. 정리 index.html 호출
    > 해당파일에 '---'로 정의된 layout 이름을 '_layout'폴더에서 찾는다.
    