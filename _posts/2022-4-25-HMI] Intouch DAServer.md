---
layout: single
title: "HMI] Intouch DAServer"
date: "2022-04-25"
categories: [HMI,PLC]
tags: []
---

Inotuch DAServer(Data Access Server)
-> Intouch의 기존 IO서버와 달리 하나의 패키지가 아닌 SMC(System Management Console)위에 설치됨.
DA Server는 기존 I/O Server의 새로운 Version.

--2003년 기준 설명
http://sammicomputer.co.kr/sub/sub04_05.php?mNum=4&sNum=6&boardid=qnaseoul&mode=view&idx=944
DA Server는 통신속도의 획기적 개선이나 Performance 측면의 개선을
목표로 둔 제품이 아니라 효율적인 I/O Server 관리와 데이터의 통합에
역점을 두고 개발된 Server입니다.

예를들어 기존 I/O Server들은 각각의 개별 Node에 설치되어 각각의
개별 Node에서만 수정과 관리가 가능했습니다.
그러나 DA Server는 하나의 Node에서 모든 분산된 I/O Server들을 통합하고
그 데이터들을 관리할 수 있습니다.
분산된 작업과 분산된 Configuration 및 Data를 하나의 Server Node에서
SMC 창을 통해 관리할 수 있도록 만든 제품 입니다.

이는 Wonderware의 새로운 제품인 Application Server의 개발 배경과도 일맥상통하는
내용으로써 분산된 Application과 개발 방법론을 하나의 Server로 집합시키기 위한
현 기술 트렌드를 반영한 최신 제품 입니다.

다음은 기존 I/O Server와의 다른 부분을 설명 드리겠습니다.
기존 I/O Server를 Install하게 되면 I/O Server EXE File이 설치가 되어지지만
DA Server는 그렇치 않습니다.
다만 DA Server를 설치하면 프로그램/Wonderware/ 에 있는 SMC(System Management Console)
에서 모든 I/O Server를 설정및 관리할 수 있습니다.

또 기존의 Topic 설정 방법도 기존의 I/O Server와 약간의 차이가 있습니다.
예를들어 ABCIP DA Server를 설정시 기존의 I/O Servers는 RS Linx가 필요한 반면
DA Server는 RS-Linx가 전혀 필요치 않으며
Control Logix에서 쓰이는 메시지 Type의 Tagname(기존 Bit체계의 어드레스가 아닌)을
직접 써서 사용을 하게 되어있습니다.

지금까지 내용이 대략적인 DA Server와 관련된 설명입니다.
참고로 기존의 모든 PLC제품에 대한 DA Server가 모두 나와있는 것은 아니고
대략 5개 정도의 DA Server만이 나와 있는 상태이기 때문에
아직까지 현장에서 범용적으로 사용되고 있진 않습니다.