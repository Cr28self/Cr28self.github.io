---
layout: post
title: 프로그래밍 언어 바인딩
subtitle : 프로그래밍 언어 바인딩을 알아보자
tags: [Compiler,CS]
author: Nayeong Kim
comments : False
---


###   바인딩(Binding)

Binding은 연관 짓는 것이다(association). 예를 들어 엔티티(Entity)와 속성(Attribute), 심벌(symbol)과 연산자(operation)를 연관 짓는 것 등을 binding이라고 한다.

### 바인딩 타임(Binding Time)

바인딩 타임은 결정되는 시점에 따른 분류로 구분지을 수 있다.

1.  언어 디자인 시점(at language design time) - 대부분의 언어에서 제어 흐름 구조, 기본 유형 집합, 복잡한 유형을 만드는 데 사용할 수 있는 생성자 및 언어론의 많은 측면들이 언어를 디자인할 때 선택된다.
2.  언어 구현 시점(at language implementation time) - 대부분의 언어 매뉴얼이 언어 구현자의 재량에 다양한 이슈를 남긴다. 예를 들어 I/O, 스택과 힙의 최대 크기 등..
3.  컴파일 시점(at compile time) - 메모리에 정적(static)으로 정의된 데이터의 레이아웃, 기계어의 상위 수준의 구성의 매핑을 선택
4.  링크 시점(at link time) - 코드 내에서 사용된 라이브러리 모듈들을 링크
5.  로드 시점(at load time) - 운영체제가 프로그램을 실행하기 위해 메모리로 불러오는 시점이다. 이때 가상 주소를 결정한다.
6.  실행 시점(at run time) - 실행 시작부터 끝까지 해당되는 영역으로 지역 변수(local variable)등을 바인딩한다.

### 정적 타입 바인딩(Static Type Binding), 동적 타입 바인딩(Dynamic Type Binding)

1. 프로그램 실행 전에 바인딩이 이뤄지고, 프로그램 실행 동안 변하지 않으면  **정적(static) 타입 바인딩**이라고 한다.

-   컴파일러 기반 언어는 인터프리터 기반 언어보다 바인딩에 대한 결정을 일찍 내리기 때문에(=static binding) 더 효율적이라고 할 수 있다.

2. 프로그램 실행 중에 바인딩이 이뤄지고, 언제든 변할 수 있으면  **동적(dynamic) 타입 바인딩**이라고 한다.

-   인터프리터 기반 언어는 컴파일러 기반 언어보다 조금 더 느린 바인딩 결정을 내리지만, 중간에 수정할 수 있으므로 더 높은 유연성을 가지고 있다.
-   컴파일 타임에 에러를 찾아내기 어렵다.
-   실행시간에 type checking을 하기 위한 비용이 든다.
