---
title: "[CS] Session과 Cookie의 차이점"
layout: single
categories: theory
tag: ['개발이론', '백엔드']
toc: true
toc_label: "목차"
toc_icon: "fas fa-list-ul"
author_profile: false
sidebar:
    nav: "docs"
---

## Session과 Cookie의 차이점은?

- **Session**은 서버에 저장하고 **Cookie**는 로컬에 저장한다.
- Session은 서버의 자원을 사용하지만 Cookie는 서버의 자원을 전혀 사용하지 않는다.

## Session

- 일정 시간 동안 같은 사용자(브라우저)로 부터 들어오는 일련의 요구를 하나의 상태로 보고 그 상태를 유지하는 기술
- 웹 서버에 웹 컨테이너의 상태를 유지하기 위한 정보를 저장한다.
- 웹 서버의 저장되는 쿠키(=세션 쿠키)브라우저를 닫거나, 서버에서 세션을 삭제했을 때만 삭제가 되므로, 쿠키보다 비교적 보안이 좋다.
- 저장 데이터에 제한이 없다. (서버 용량이 허용하는 한에서)
- 각 클라이언트에 고유 Session ID를 부여한다. Session ID로 클라이언트를 구분해 각 요구에 맞는 서비스를 제공

## Cookie

- HTTP의 일종으로 사용자가 어떠한 웹 사이트를 방문할 경우, 그 사이트가 사용하고 있는 서버에서 사용자의 로컬에 저장하는
  작은 기록 정보 파일
- 이름, 값, 만료일(저장기간), 경로 정보로 구성되어 있다.
- 클라이언트에 총 300개의 쿠키를 저장할 수 있다.
- 하나의 도메인 당 20개의 쿠키를 가질 수 있다.
- 하나의 쿠키는 4KB(=4096byte)까지 저장 가능하다.

