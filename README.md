# java-calculator-precourse

# 기능 요구 사항

#### 입력한 문자열에서 숫자를 추출하여 더하는 계산기

### 기능 
  - 문자열 입력 받기
    - '덧셈할 문자열을 입력해주세요.' 출력
    - 다음 줄에 문자열 입력 받기
  - 숫자를 추출하기
    - 쉼표 또는 콜론을 구분자로 가지는 문자열, 커스텀 구분자 지정 가능(//와\n사이에 위치하는 문자)
    - 입력 받은 문자열에서 숫자를 추출하기
    - 추출한 숫자를 배열에 저장하기
  - 더하기
    - 배열의 숫자를 모두 더하기
  - 결과 값 출력하기
    - '결과 :'을 출력한 후 더한 숫자를 출력하기

### 클래스
  
- InputManager 입력 클래스
  - [X] 입력하라는 메시지 출력 함수
  - [X] 문자열 입력 받는 함수
  - [X] 입력 시 발생 가능한 예외 처리

- NumberExtractor 숫자 추출 클래스
  - [X] 커스텀 문자열 추출 함수 
  - [X] 커스텀 구분자를 제외한 문자열을 반환하는 함수
  - [X] 숫자를 추출해서 배열에 저장하는 함수
  - [X] 커스텀 구분자를 포함하여 숫자를 추출해서 배열에 저장하는 함수

- Calculator 계산기 클래스
    - [ ] 더하기 함수
    - [ ] 결과값 출력 함수

- Application 메인 클래스
  - [ ] 입력 클래스 생성
  - [ ] 숫자 추출 클래스 생성
  - [ ] 계산기 클래스 생성

# 예외 처리

-[X] **IllegalArgumentException** : 사용자가 잘못된 값을 입력한 경우

-[ ] **InvalidDelimiterException** : 구분자가 쉼표나 콜론, 커스텀 구분자가 아닐 경우

-[ ] **NegativeNumberException** : 문자열이 양수가 아닐 경우

-[X] **EmptyException** : 아무 것도 입력되지 않을 경우