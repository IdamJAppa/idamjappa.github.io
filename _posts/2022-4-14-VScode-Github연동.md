---
layout: posts
title : "VSCode] VSCode-Github연동법"
categories : [VSCode]
---
1. VsCode 설치

2. Git 설치(OS, bit에 맞게 설치)
    - 설치 시 Default Editor는 VsCode로 지정
        * 다른걸 써도 되겟지만, 굳이..

    - 설치 후, 기본정보 설정
        > git-cmd.exe 실행
        > 사용자 이메일 / 이름 설정
            >> git config --global user.email "이메일주소"
            >> git config --global user.name "사용자이름"
            
    * Portable Git을 설치 해봤는데, VsCode가 못 가져오는 것같다. 추가 확인필요함

3. VsCode 실행
    - View >> SCM(Source Control Manager) 실행
       [Ctrl. + Shift + G]

    - 'Clone Reppsitory' 클릭
    - VsCode와 연결을 원하는 내 Reposity URL 입력
    - 로컬에 저장 할 폴더 지정
        > GitHub 리포지토리에서 로컬폴더에 소스 Pull해옴
    - VsCode 연결완료