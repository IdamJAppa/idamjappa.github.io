---
layout: posts
title: "Jekyll] MMinial테마 플로우 따라가봄"
date: "2022-04-22"
categories: [Jekyll]
tags: []
---

0. 전제
    - Jekyll Minimal-Mistake 테마가 로컬 혹은 Github내에 디플로이 된 상태
    - 기본 블로그 설정(_config.yml) 완료상태
    - 파일별 내부구동 설명은 파일 참고.

    > index.html 실행
    > _layouts 폴더의 home.html 호출
    > index.html 미종료
    >> home.html에서 _layouts 폴더의 archive.html 호출
    >> home.html 미종료
    >>> archive.html에서 _layouts 폴더의 default.html 호출
    >>> archive.html 미종료
    >>>> default.html 에서 _includes 폴더의 head.html, /head/custom.html 호출
    >>>> head.html, cusom.html 모두 처리 후 _includes 폴더의 
         skip-links.html, browser-upgrade.html, masthead.html 호출
    >>>> default.html 내에서 메인페이지의 head, master head 완성
    >>>> liquid문법 'content' 통해 default.html을 호출한 archive.html로 돌아감
    >>> archive.html에서 sidebar.html 호출
    >>> sidebar.html에서 author-profile.html 호출
    >>> archive.html에서 liquid문법 'content' 통해 archive.html을 호출한 home.html로 돌아감
    >>> archive.html 종료 
    >> home.html에서 liquid문법 'content' 통해 home.html을 호출한 index.html로 돌아감
    > index.html 종료 (아무것도 없음)
    >> home.html로 돌아와서 '/_post'폴더의 .md 포스트들을 archive-single.html에 넣어서 불러옴
    >> paginator.html 실행
    >> home.html 종료
    >>>> 미종료된 default.html로 이동
    >>>> footer.html, scripts.html 수행후 페이지 완성
