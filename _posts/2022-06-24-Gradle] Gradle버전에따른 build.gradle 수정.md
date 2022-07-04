---
layout: single
title: "Gradle] Gradle버전에따른 build.gradle 수정
date: "2022-06-27"
categories: [Gradle, SpringBoot]
tags: []
---

Gradle 7.0 이상버전 부터 
build.gradle 내 사용되는 명령어가 변경됨

기존 : compile, testCompile, runtime, testRuntime
변경 : implementation, testImplementation, runtimeOnly, testRuntimeOnly

참고링크
https://velog.io/@g0709-19/Gradle-Could-not-find-method-compile-%ED%95%B4%EA%B2%B0-%EB%B0%A9%EB%B2%95