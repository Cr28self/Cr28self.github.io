

---
layout: post
title: 프로그래밍언어론 - 언어의 변천
subtitle : 언어의 종류 및 특징을 알아보자
tags: [CS, Compiler]
author: Nayeong Kim
comments : False
---



# Chapter2 - 언어의 변천

> PL은 **프로그램을 저장할 수 있는 능력을 가진 컴퓨터에 대한 계산 과정을 기술할 수 있을때부터** 의미함.
따라서 **PL의 역사는 1940년대부터 시작된 프로그램 저장 컴퓨터의 발전과 함께한다고** 할 수 있음.
> 

## [ 디지털 컴퓨터 이전의 언어 ]

### 최초의 알고리즘

- **찰흙판**, BC 1500 – 3000, 바빌론 근처 메소포타미아
    - 60진법 사용 (현재 시, 분, 초 개념에 사용), 부동 소수점( 정수 ) , 가감승제 가능 ( 사칙연산 )
    - 대수학 방정식 해결 ( This “ is a procedure( function ).” 표현 사용)
- if x < 0 then branch 개념 없음 (음수, 0 개념 없음) ( 조건문 개념 없음 )
- 여러 가능성을 표현하기 위해 필요한 만큼 알고리즘 반복 작성
    - 주어진 **문제가 해결될때까지** **여러번 반복작성함.**
    - 우수한 표기법이었음

### 유클리드 알고리즘 ( 호제법 )

- B. C. 300 B. C. 300년, **최대공약수 알고리즘** (모국어 사용)
- 수에서 **0 개념 없음**, 수 **1이 제수로 인식되지 않았음**
- 특수한 경우 반복시킴
- 바빌로니아 사람들 보다 별로 진보되지 못함

### Charles Babbage ( 1792 - 1871 ) <산업혁명 시기>

- **Difference Engine**
    - 계산 처리를 위한 기계
    - 유한 차(finite difference) (finite difference)의 원리를 기본으로 함
        - **차분 해석 기관**이라고 한다. ( **차이를 분석하는… , 증기기관 원동력**으로. )
- **Analytical Engine** : 현 디지털 컴퓨터의 원리 포함
    - 현재 컴퓨터와 유사한 구조
    - 프로그램과 자료를 주기억장치에 저장시키는 저장 개념 없음 (연산카드, 변수카드 사용)
- **Ada Augusta**(Charles Babbage 조수)
    - 최초의 컴퓨터 프로그래머 (Analytical Engine 프로그래머)
    - 그녀의 이름을 따 Ada언어 만들었다

- **Ada 언어**
    - 미 국방성에서 사용됨
    - **진정한 객체 지향 언어**
    - 이 이후에 완전히 새로운 언어가 만들어지지 않았다.
        - 전부다 파생되는 식으로 언어가 만들어졌다.
- **Ada의 ‘알고리즘 분석’에 대한 견해**
    
    > “거의 모든 계산에서 성공적인 수행을 할 수 있는 매우 다양한 배치 방법들이 가능하다.
    그리고 이들 배치 방법을 선택하는데 있어서 **계산을 수행하는 기계 목적에 맞도록 여러
    가지 고려해야 할 점**들이 있다. 한 가지 **중요한 고려 대상**은 **계산하는데 필요한 시간을
    최소로 줄이는 배치 방법**을 선택하는 것이다”
    > 
    - **최대한 빨리 계산하는 방법을 선택**

---

---

## [ 1930 - 1940 년대 ]

- 프로그래밍 표기에서 창조적인 것들이 급격하게 증가
    - Zuse의 Plan Calculus
    - Turing의 Turing Machine
    - Church의 Lambda Calculus
        - 후에 LISP언어의 기본이 된다.
    - Aiken의 Mark-I ( 1942 )
        - 기계적인 컴퓨터
        - 이와 대비되는 전자적 컴퓨터인 ABC컴퓨터
            - 컴퓨터가 만들어진 후 15년 뒤 PL이 만들어졌음
                - 그 전에는 계속 기계어 사용햇었음
    - **von Neumann의 Flow Diagrams**
        - **프로그래밍 내장 방식 ( Stored Programming )**
        - **명령어 저장 → 하나씩 꺼내서 실행**

- 이러한 연구들이 디지털 컴퓨터의 초기 개발자에게 알려지지 않았음
    - **초창기에는 Hardware적인 언어를 사용**했으므로…

---

---

## [ 주요 고급 언어의 계보 ( 1950년대부터 ) ]

![Untitled](Chapter2%20-%20%E1%84%8B%E1%85%A5%E1%86%AB%E1%84%8B%E1%85%A5%E1%84%8B%E1%85%B4%20%E1%84%87%E1%85%A7%E1%86%AB%E1%84%8E%E1%85%A5%E1%86%AB%20288f96aa62274cc5a63be0062523aaf9/Untitled.png)

---

## [ 1950년대 - 최초의 프로그래밍 언어 ]

### 1950년대 초반

- 이 당시에 **프로그램 저장방식의 출현**
- 이 당시에 프로그램은 주로 기계어로 작성되었으나, 뒤이어 어셈블리 언어가 탄생하여 기계어 코드를 대신해서 사용하게 되었다.
- **어셈블리 언어 ( 기호와 연상기호 사용 ) — < 저급언어 >**
    - **기계 의존적**임
    - **자연어와는 차이가 큰 구문**을 사용함

---

## [ 고급 프로그래밍 언어 ]

### 1950년대 중반 — FORTRAN 탄생

- 1954~75, John Backus
- **최초의 고급 프로그래밍 언어**
    - 많은 새로운 특징 탄생
        - 배열, 제어 변수를 쓰는 반복구조, 조건문에 의한 분기문, 부 프로그램에 관한 특징
            - 나중에 만들어진 언어들의 모범이 되었다.!!
- 본래 과학적 계산 위한 목적
- 오늘날까지도 개선된 버전으로 과학 분야에서 사용
- 이들은 다목적 프로그래밍을 위해 다른 언어의 새로운 특성을 추가하는 식으로 여러 버전이 탄생했음
- **FORTRAN이 긴 생명을 가질  수 있었던 이유??**
    - Fortran컴파일러가 **다른 고급언어에 비하여 효율적 기계어 코드를 생성**하므로..
        - **사람이 직접 작성한 기계어 코드보다는 덜 효율적**이었음에도 불구하고 
        **프로그램 작성 속도에 있어서 효율성**이 이를 전부 포용할 수 있었으므로 
        < 고급 언어로 프로그램을 작성하는게 훨씬 빠른 결과를 제공한다는 것을 알게 되었다>

### 1950년대 후반에 등장한 언어

- **Cobol ( 1959 ~ 60 )**
    - 미 국방성에서 개발
    - 은행, 기관들이 **사무처리를 위해 채택** ( 상업 자료 처리용 , 사칙연산 계산 위주 )
    - 자료를 구성하는데 **레코드 구조를 도입**
    - **자료구조와 실행 부분을 분리**
- **Algol 60 ( 1958 ~ 60 )**
    - 알고리즘을 기술하기 위한 일반적인 표현 언어
    - 연구용 및 실질적인 응용 목적 ( 범용 )
    - Pascal, C, Modula-2, Ada 등 상용되는 대부분의 언어들은 Algol의 파생어.
    - **블록 구조를 쓰는 언어들을 위하여**
        - **Stack기반으로 하는 실행 환경 도입**,
    - **구문을 정의하기 위하여**
        - **BNF환경 최초 사용**
    - 프로그래밍에 **양식의 자유화 ( free-format )**, **구조적 명령문**, **begin-end블록**,
    **변수의 타입 선언**, **recursion**, **값 호출 ( call -by-value )**개념 소개
    
    > 위에서 소개한 3가지 언어는 전부 폰노이만 구조 기반 ( Fortran, Cobol, Algol 60 )
    > 
    
    > 밑에 2개 언어는 함수의 수학적 개념을 기저로 한다.
    > 
    
- **LISP ( 50년대 후반 )**
    - J.McCarthy
        - MIT 대학교
    - 기호 연산, 리스트 처리용
    - 리스트 구조와 함수의 응용을 기본으로 하였음.
        - **인공지능분야**에서 사용
        - **배열형태로 나열해서 연산**
        - **수학적 함수 사용**
    - **초기의 인공지능 언어**
    - **획일적인( 통일된 ) 자료구조**
    - **Heap / 가비지 컬렉터 방식 소개**
        - 실행시간의 기억장소 배당 방법을 지원하려고
            - run-time 기억장소 할당 제공을 위해
        - 더이상 사용되지 않는 기억장소를 자동으로 재생하는 방식도 소개
    - **많은 의사 결정 시스템이 LISP로 작성**됨
    - **폰노이만 구조와는 다른 연산 방식**
        - 기존의 컴퓨터에서 효율적으로 실행 어렵
    - **recursion의 원조**
    - I**PL5에서 파생됨**

- APL ( 50년대 후반 60년대 초 )
    - 배열과 행렬을 포함하는 **수학적 연산을 쉽게 프로그래밍하기 위한** 언어
    - IBM에서 제작
    - 기능적인 style, 반복구조 자동 제공 연산자 채택
    - **제어 구조 없음**
    - **프로그램 결과 예측 불가능**
        - **인터프리터 사용**
    - **이해 어렵..**
    - **그리스 기호 사용**

---

---

## [ 1960년대 — 프로그래밍 언어의 폭증 ]

- 초기 언어의 성공 → 언어 개발 몰두 → 언어의 폭증 ( 특별한 관심 분야나 목적을 위한 언어 )
- 수많은 언어의 생성 시기
- 이 시기에 개발된 대부분 언어는 소멸되었으나 일부 언어는 PL발전에 큰 공헌

- **좀더 일반적이고 보편적인 언어, 만들기 위한 프로젝트** : IBM의 PL/I 프로젝트

### PL/I(63~64년) : IBM Project(IBM 360 시리즈에 사용 계획)

- **새로운 개념 추가 (병행성, 기억 장소 할당, 예외처리)**
    - 이전에 개발했던 Fortran, Cobol, Algo60의 장점 모두 수용
- IBM의 막강한 지원이 있었으나 많은 문제점 내포
    - 번역기가 크고 작성이 어려움 / 실행 효율 저하 / 배우기 어려움, 오류 발생 유도
    - 언어 특성들의 상호 작용으로 인한 신뢰성 저하

### Algol68(63~68년) — C언어의 큰 영향

- **Algol60 + 타 언어의 여러 기능 + 표현력 있고 일관된 구조**
    - **Algol60 개선한 형태**
- **새로운 특징을 독자적으로 개발**
    - **다른 언어에서 모방하지 않았음**
- 이론적으로 **일관성 갖는 구조를 만들어 표기 할 수 있게 발전**시켰음
- 일반적인 **형 시스템 포함** 시킴
- **임의의 제한을 두지 않는 수식 위주의 직교성 강조 ( 직교 언어 
)**
- Algol68 위원회는 언어 기술하기 위한 정의를 내렸음 
→ 새로운 용어 과다 사용
    - 읽기에 벅찬 내용이 되었다.
- 디자인 일관성, 파일 시스템, 실행 환경 → 우수
- **범용 컴퓨터 사용 불가능 (비판 → 소수 구현)**

## [ 1960년대 — 프로그래밍 언어의 폭증 ] 시기에서 
언어의 발전에 공헌한 언어들

### Snobol

- 벨 연구소, R. Griswold가 개발
- **최초의 문자열 처리 언어**, **복잡하고 강력한 패턴 매칭** 기능

### Simula67

- Nygaard & Dhal(Norway) 개발
- **객체 지향 언어(클래스 개념 최초 도입)**
    - **최초의 객체 지향 언어!!**
- 60년대 초 고안되었던 **Simula를 기본으로 하여 Algol60을 포함**시켰다.
- 시뮬레이션 목적

### Basic

- 1964년 J. Kemeny & T. Kurtz(Dartmouth Univ.) 개발
- 새로운 시분할 시스템을 위한 간결한 언어로 개발하였음
- **마이크로 컴퓨터 이식 (교육용, 사무처리용, 가정용으로 널리 보급되었음)**
- **Basic**은 하나의 언어가 아닌 **언어군**에 속한다.
    - ( **두개의 Basic을 ANSI가 표준화** —> 1978 ‘minimal Basic’,   1988 ‘Standard Basic’)
- 후에 나온 Basic : 제어 구조, 변수 선언, 프로시저 추가
    - 그러나 현재까지 **초기 Basic이 간결성 때문에 더 널리 사용**되고있다.

---

---

---

## [ 1970년대 — 간결성, 추상화, 연구 사항 ]

- 60년대 혼돈 후 → **언어 설계자들은 <간결성>과 <일관성>을 추구**
    - **간결하게 —> 추상화 개념**
    - Niklaus Wirth : Algol 68 디자인에 반발 (방대성)
    - Algol W 제안

### < 1970년대 초반에 등장한 언어 >

### Pascal ( 1971 ) : Niklaus Wirth

- 작고, 간결하고, 효율적이고, 구조적이며, 프로그래밍 교육용
    - **구조적 프로그래밍 언어**에 속함
    - **Algol의 개념으로부터 정제**하여 만들었음
- **소규모**로서 **분리 컴파일**, **유용한 문자열 조작**, **입출력 기능** → **삭제 또는 축소**
    - 실제 **응용에도 성공적**이었음

### C언어 ( 1972 ) : 데니스 리치

- **Algol의 한계성을 극복한 사례**
- **Pascal과는 다른 각도의 간결성**
    - **수식 위주로 국한**하여 **형 시스템의 복잡성 & 실행환경 축소**
     → **하드웨어에 좀더 가까이 접근**할 수 있게 되었다.
        - 이러한 이유 ( 기계 접근성 강화 )로 **C언어는 고급 언어와 상반되는 개념**이 있음
            - **중급 프로그래밍 언어로 분류**
- OS 프로그래밍에서 사용되기도 했음
    - **OS프로그래밍용 : Bliss, Forth**
- UNIX
    - C언어로 작성된 운영체제
    - 대성공
        - C언어 대중화

### C언어와 Pascal의 공통된 성공 요인

- 그 언어들이 가지는 **간결성과 전체적인 디자인 일관성이** 성공적인 요소가 되었다.
- 더 나아가 **PL을 디자인하는 새로운 개념으로 공헌한 셈**이 되었다.

---

### < 1970년대 중,후반에 등장한 언어 >

- PL디자이너들은 **<자료 추상화>, <병행성>, <증명>** 등의 매커니즘을 집중적으로 시도하게 되었다.

### CLU

- **추상화 기법**을 위한 일관성 있는 접근 방식 - 자료 추상화, 제어 추상화, 예외처리
    - 자료 추상화 : cluster (Simula의 class와 유사)
    - 제어 구조 : iterator - 일반성
    - 예외처리 : Ada와 비슷한 구조 제안

### Euclid

- **Pascal을 개선**한 언어
- Pascal의 단점인 **이명(aliasing) 개선**, 자료형의 추상화, 프로그램 증명 보조 추가
- 프로그램의 형식적 **검증(증명)**을 목적으로 한 최초 언어

### Mesa

- **병행성** 강조
- Pascal 구조에 모듈 구조, 예외처리기, 병행성, 병렬 프로그래밍의 개념 추가
- 시스템 프로그래밍용 → Modula-2 메커니즘 고안에 지대한 영향

---

---

---

## [ 1980년대 — 통합과 새로운 방향 ]

- 8bit PC가 생성되던 시기

- **Ada언어 등장** ( **개념 통합** )
    - 이전에 생성한 언어들의 개념들이 통합됨
- **함수형 언어에 새로운 관심** 부여 — 스킴 ( Scheme ), ML( Meta Language ) 개발
- **논리형 프로그래밍 언어** — **Prolog** 등장
- 객체 지향 언어에 대한 활발한 연구 및 개발

### Ada

- J. I hbi h Ichbiah Team ( 미 국방성의 공모작 수정)
- **자료 추상화, 타입 메커니즘(package), 병행 처리(task), 예외처리기 도입**
- 디자인이 섬세하고 상세함, 사용 급증
- 단점 : 복잡 방대 (제 2의 PL/I 가능성)
    - 수많은 기능이 존재했다.
    - **이로 인해 일반 컴퓨터에서 사용하지 X**
        - **슈퍼컴퓨터에서..**
- **이후에 새로운 언어가 만들어지지 X**
    - **C언어에서 파생되는 형태로 만들어짐**

### Modula-2 : 1982-88, Modula 언어를 기본, 운영체제 구축용( N. Wirth)

- **Pascal의 디자인에 결점 보완**(당시 실험적 언어)
- 추상화, 부분적 동시처리 개념, 교육 목적으로 인기
- **내장형 시스템 프로그래밍 목적 ( Embeded )**: 하드웨어 접근이 용이한 다목적 언어
- 가능한 한 소규모의 간결한 언어로 시도 → 예외처리 기능 등 제외

### Prolog

- 논리형 언어
- 인공지능 분야에서 많이 사용

### SETL

- 집합론을 프로그래밍 언어로 시도한 것
    - 미적분, 수학의 교육 모델로 사용
- 구현 결핍 → 사용 어렵

### Smalltalk

- 객체 지향 접근 방식으로 일관된 객체 지향 언어의 모범 케이스

### C++

- C언어를 확장한 객체지향 언어

### Eiffel

- Pascal에 가까우면서 일관성 있는 객체지향 언어

### < 1980년대 등장한 함수형 언어 >

### Scheme

- Lisp 언어 개정
- Lisp의 한 버전
- Lisp보다 획일적이고, lambda calculus에 가깝게 설계됨

### Common Lisp

- 표준으로 규정됨
- Lisp의 또다른 버전임

### ML

- 앞서 나온 기존 함수형 언어와는 상당히 다른 형태
    - Pascal과 비슷한 문법
    - 타입 검사 ( type-checking )도 Pascal과 비슷
    - Pascal보다 훨씬 유연성 있음

### Miranda

---

---

---

## [ 1990년대 — World Wide Web 프로그래밍 ( JAVA ) ]

- 제 4세대 언어
    - DB시스템을 위해 만들어진 명령어
        - SQL, 델파이, Lotus
    - 실용성 크다
    - 응용문제를 빠르게 구현 가능
    - 실사용자가 직접 프로그래밍 가능
    - 데이터베이스를 쉽게 처리가능

- 4세대 언어들이 다양하게 대두되었음

- 명세 언어
    - 사용자가 원하는 바를 서술하면 시스템이 요구 사항을 구현해 줄 수 있는 언어

- HTML , JAVA 등장

- 스크립트 언어 ksh
    - sh + 변수, 제어문, 함수 ⇒ 하나의 완벽한 프로그래밍 언어

- WWW이 널리 사용됨에 따라 Perl 언어 ( sh + awk 형태 ) 의 사용이 급격하게 상승함
    - CGI프로그래밍에 이상적인 언어임!!
- CGI
    - 웹 서버상에서 사용자 program을 동작 시키기 위한 조합

### JAVA

- James Gosling
- C++ 기반 : 많은 구조 삭제, 일부 구조 변경, 일부 구조 추가
    - 기본 자료형 : 스칼라 형
    - 논리형 제공 ( 산술 연산에 사용 불가 : C,C++와 구별 )
    - 부 프로그램 제공 X ⇒ class method 제공
    - 동시성 제공 — Thread
    - 가비지 컬렉터
    - 단일 상속 ⇒ 다중 상속 변칙 사용 ( 인터페이스 제공 )
    - 묵지석 형 변화 — 확대형 변환
    - 중간 언어 제공 ( 이식성 up )
    - Java 애플릿 — client에서 실행
    - C++의 포인터 기능 삭제
        - 대신 참조형 제공
            - 포인터  : 기억 장소 지시
            - 참조형 : 객체 지시
    - C++의 강력함과 유연성 제공
    - C++보다 규모는 작아지고, 더 간결하고, 신뢰성(안전)이 증가된 언어
- 초기 응용 분야 목표 : 제품 장치를 위한 내장 시스템
- Java의 응용 분야가 확장됨 ⇒ Web 프로그래밍 (C/C++결점 보완)

---

---

---

## [ 프로그래밍 언어의 세대론과 미래 ]

### 프로그래밍 언어의 세대 구분 ( 견해에 따른 2가지 분류 )

- 제 1세대 — 어셈블리 언어 / 기계어
- 제 2세대 — 비구조형 고급 언어 / 어셈블리 언어
    - Fortran, Cobol, Basic 등 : 비구조형 언어
- 제 3세대 — 구조형 고급 언어 ( begin…end 개념, 블록 개념 )  / 고급 언어
    - PL/I, Pascal, C 등 : 프로시저 위주의 고급 언어
- 제 4세대 — 화일처리(SQL등) / 화일처리(SQL등)
- 제 5세대 — 초고급 언어 / 초고급 언어
    - Prolog, SETL

---

---

## [ 언어의 변천 Diagram ]

![Untitled](Chapter2%20-%20%E1%84%8B%E1%85%A5%E1%86%AB%E1%84%8B%E1%85%A5%E1%84%8B%E1%85%B4%20%E1%84%87%E1%85%A7%E1%86%AB%E1%84%8E%E1%85%A5%E1%86%AB%20288f96aa62274cc5a63be0062523aaf9/Untitled%201.png)

---

---

## [ 프로그래밍 언어의 세대론과 미래 ]

### 소프트웨어 위기의 극복

- 언어적 기술보다는 **<조직적인 방법>으로 해결**
    - **기존 코드의 재사용 증대**
    - **이식성 증대**
    - **문법 위주의 에디터** ( VSCode, IntelliJ 등 자동완성 지원 )를 사용하여 생산성 높임
- **언어 설계의 미래**
    - **Hardware와 컴퓨터 구조의 발달에 의해 영향** 받음
    - **새로운 언어의 출현보다는 기존의 언어들을 갈고 닦아, 언어 설계에 대한 이해를 점진적으로 증가시키는 방향으로 예상**됨