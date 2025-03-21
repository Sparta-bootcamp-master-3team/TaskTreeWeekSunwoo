
# GrammarProblems
## 소개
> 심화 문법 주차 개인 과제로 필수 문제 3문제와 도전 문제 1문제를 구현했다. 요구사항에 맞게 알맞은 문법을 사용해서 구현했다.

## 기술
- 개발환경: Xcode, macOS, Command Line Tool
- 언어: Swift
  
## 설명
### 필수 문제 1번
- 두 개의 Int 값을 파라미터로 받고 하나의 String 값을 반환하는 클로저를 만들고 실행
- 위 클로저와 동일한 타입의 클로저를 파라미터로 받는 함수 생성 후, 실행
> ![스크린샷 2025-03-19 오후 5 59 27](https://github.com/user-attachments/assets/1d1bad1b-6814-4534-a499-d45f73bba624)

### 필수 문제 2번
- 고차 함수 map을 사용하여 정수 배열값을 입력값으로 받아서 문자열 배열값으로 출력하는 코드로 변환
- 고차 함수 filter, map을 사용해서 정수 배열값을 입력값으로 받아서 문자열 배열값으로 출력하는 코드로 변환
- map과 비슷한 역할을 하는 고차함수 myMap을 커스텀해서 만들고 실행
  - 형변환을 하기 위해 String타입의 빈 배열을 선언하고 반복문을 사용하여 파라미터로 받은 값들을 새로운 배열에 삽입하고 반환
> ![스크린샷 2025-03-19 오후 5 59 40](https://github.com/user-attachments/assets/785dbf10-6cd6-4fc6-afcd-ad8a89e8b73d)

### 필수 문제 3번
- Int 배열의 홀수번째만 반환하는 함수 a를 만들고 실행 (조건은 삼항연산자를 사용)
- 함수 a에서 타입만 Int에서 String으로 변환한 함수 b를 만들고 실행
- 제네릭을 사용하여 함수 a, b를 하나의 함수로 대체하는 함수 c를 만들고 실행
- 함수 c 를 기반으로 파라미터의 타입을 'Numeric 프로토콜'을 준수하는 배열인 함수 d를 만들고 실행
> ![스크린샷 2025-03-19 오후 5 59 49](https://github.com/user-attachments/assets/4e43853a-3c13-4ddb-8fdf-06d5bf413a8c)

### 도전 문제
- Engine이라는 기본 클래스를 선언 후 값이 바뀌는 것을 보기 위해 print값을 가진 메서드 engineType 설정
  - Engine을 상속받는 ElectricEngine이라는 클래스 생성 후 메서드 engineType을 재정의
  - Engine을 상속받는 HybridEngine이라는 클래스 생성 후 메서드 engineType을 재정의
- 기본 Class Car를 만들고 파라미터와 메서드 선언
  - 파라미터 brand, model, year 모두 String 타입
  - engine: 클래스 Engine을 선언해서 커스텀 타입으로 가짐
- Car를 상속받는 ElectricCar를 선언
  - ElectricEngine 타입의 Engine을 사용
- Car를 상속받는 HybridCar를 선언
  - HybridEngine 타입의 Engine을 사용
  - 엔진을 바꿀 수 있는 switchEngine(to:)이라는 메서드 선언
- HybridCar 인스턴스를 생성하고, switchEngine(to:) 를 호출하여 서로 다른 타입의 엔진으로 교체하는 코드를 실행
> ![스크린샷 2025-03-19 오후 5 59 58](https://github.com/user-attachments/assets/e6b0f088-a125-485a-b21b-8fb4ddc7386f)

## 프로젝트 구조
```
GrammarProblems/
│── Challenge
│       └── ChallengeProblem.swift
│── Essential
│       │── Problem1.swift
│       │── Problem2.swift
│       └── Problem3.swift
└── main.swift  
```
