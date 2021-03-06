# 2
## 문제 해결 알고리즘
1. 문제를 읽고 이해한다.
2. 문제를 익숙한 용어로 재정의 (이거는 굳이 안해도 될듯함)
3. 어떻게 해결할지 계획을 세운다.
4. 계획을 검증한다.
5. 프로그램으로 구현
6. 어떻게 풀었는지 돌아보고, 개선 방법 찾는다. (이거는 시간 남으면)
### 1. 문제를 읽고 이해하기
* 모든 공통 실수는 문제를 잘못 읽는 실수다.
### 2. 재정의와 추상화
* 자신의 언어로 문제를 풀어쓴다.
* 문제의 추상화가 필요하다.
  * 여기서 추상화란 수학적/전산학적 개념으로 옮겨 표현하는 과정
### 3. 계획 세우기
* 사용할 알고리즘, 자로구조 선택
### 4. 계획 검증
* 알고리즘이 잘 돌아가는지, 자료구조가 적절한지를 확인한다.
### 5. 계획 수행하기
* 구현
### 6. 회고하기
* 다시 풀어보면 더 좋은 방법을 찾을 수 있다.
* 만약 오답이였으면, 오답 노트를 적어라
### 문제를 풀지 못할 때
* 참고해라 다른 답을
  * 하지만 참고하고, 내가 접근했던 방법을 확인해라
## 문제 해결 전략
어려운 문제일수록 다양한 방법을 시도해야 된다.
### 직관과 체계적인 접근
* 문제와 답의 구조에 대한 직관의 중요성
* 해당 문제를 해결하는 알고리즘이 대략적으로 어떤 형태를 가질지를 짐작할 수 있게 해준다.
* 직관을 발달시키려면 막막한 문제들을 해결하며 실력을 늘려야된다.
### 체계적인 접근 위한 질문
* 비슷한 문제를 풀어봤나?
  * 비슷한 문제여도 응용 문제를 많이 풀어봐라
* 단순한 방법에서 시작할 수 있을까?
  * 무식하게 푼다 -> 리팩토링의 반복
* 문제를 푸는 과정을 수식화할 수 있을까?
  * 손으로 풀고, 그 공식을 알고리즘으로 만들 수 있다.
* 문제를 단순화할 수 없을까?
  * 좀더 쉬운 문제를 풀고, 어려운 문제를 풀어는것도 좋다.
  * 더 단순화 방법
    * 제약 조건을 없에본다.
    * 변수의 수를 줄인다.
    * 다차원의 문제를 1차원으로 변경해서 풀어본다.
* 그림으로 그려보자
  * 문제에 관련된 그림을 그려본다.
* 수식으로 표현할 수 있나?
  * 평문을 수식으로 표현하면 도움이 될 때가 있다.
* 분해해보자
  * 제약 조건을 분해한다.
* 뒤에서부터 생각해서 문제를 풀 수 있을까?
  * 사다리타기를 예로 들어보면 밑에서부터 위로 올라가는 것이다.
* 순서를 강제로 정해보자
  * 순서를 정해준다. (내 마음대로)
### How to solve it (번역한거였음)
문제 해결에 있어 단양한 전략들을 나열한다.
# 3
## 코딩의 중요성을 간과하지 말라
* 프로그래밍 대회 입상자의 코드는 대부분 간결하고 이해하기 쉽다.
## 좋은 코드를 작성하는 방법
* 간결한 코드 작성
  * 코드가 짧을수록 오타가 줄어든다.
  * 매크로를 사용하면 변수 실수가 없을 수 있다. (그래도 사용하지 말자...)
* 적극적 코드 재사용
  * 코드를 모듈화해라
* 표준 라이브러리 공부하기
* 항상 같은 형태로 프로그램을 작성하기
  * 검증된 코드를 작성하는걸 노력해라
* 일관적이고 명료한 명명법 사용하기
  * 변수명, 함수명
* 코드와 데이터 분리
  * ex ) monthName 배열 사용, daysIn (월 마다 일 수)
## 자주 하는 실수
* 산술 오버플로
* 배열 범위 밖 원소에 접근
* 일관되지 않은 범위 표현 방식 사용하기
  * 닫힌 구간
    * [2, 12]
    * = 2 <= i <= 12
  * 열린 구간
    * (2, 12)
    * = 2 < i < 12
* 최소, 최대 예외 잘못 다루기
* 연산자 우선순위 잘못 쓰기
  * 비트단위 연산자는 우선순위가 낮다.
* 너무 느린 입출력 방식
  * cin, cout, scanner
* 변수 초기화 문제
  * 두 번째 입력을 생각하지 않은경우
## 디버깅과 테스팅
* 디버깅에 관하여
  * 프로그래밍 대회에서는 소스코드를 눈으로 디버깅이 가능하다. (짧음)
  * ACM-ICPC 의 경우는 한 명이 코더기 때문에 더 가능
  * 작은 입력값으로 간단하게 확인
  * 단정문을 쓴다. (주어진 조건이 거짓일 때 오류, 강제종료)
  * 계산 중간결과 출력
* 테스트에 관하여
  * 스캐폴딩 기법
    * 맞왜틀인 경우에 사용한다.
    * 답안을 검증하는 코드를 작성한다.
    * 대회에서는 라이브러리를 사용 못해서 거의 힘들다
      * 표준 라이브러리로 정렬한 값, 내가 구현한 정렬의 값 비교
## 변수 범위의 이해
### 산술 오버플로
컴퓨터는 수학자들이 만든 기계이며 수학에 따라 움직인다.
* 값의 제한이 있다.
* 예상과 다르게 움직이는 경우가 있다.
  * 흔한 원인중 하나가 산술 오버플로우다.(arithmetic overflow)
    * 대부분의 프로그래밍 언어는 산술오버플로우가 나는걸 알려주지 않다. (일일이 체크하면 오버헤드가 크다.)
    * 프로그램 논리의 정확성에만 집중하다보면 산술 오버플로가 나타날 수 있다는걸 모를 수 있다.
#### 너무 큰 결과
32 비트 자료형의 범위에 64 비트 정수를 사용하면 넘어간다.
#### 너무 큰 중간 값
lcm(최소공배수)를 구하는 경우 gcm(최대공약수) / lcm 이다.

40억 / 10억 이라고 했을 때, 기대 결과는 4다.

하지만 40억이 산술오버플로를 일으킨다.

그래서 원하는 값이 나오지 않는다.
#### 너무 큰 '무한대'값
흔히 최단거리를 구하는 알고리즘에서 사용하는 INF 값이 연산이 일어나 산술 오버플로를 일으킬때가 있다.
#### 오버플로 피해가기
* 더 큰 자료형 사용
* 곰셈의 교환법칙을 이용해 나눗셈을 먼저 연산한다.
#### 자료형의 프로모션
보통 연산자는 피연산자를 두 개 받는다.

컴파일러들은 대게 이 피연산자의 자료형을 동일하게 만들고 연산한다.

이를 *프로모션*이라고 한다.

C++ 의 과정을 설명한다.
1. 한쪽은 정수, 한쪾은 실수형인 경우: 정수형이 실수형으로 변환된다.
2. 양쪽 다 정수형이거나 양쪽 다 실수형일 경우: 넓은 범위를 갖는 자료형으로 변환된다.
3. 양쪽 다 int 보다 작은 경우: 양쪽 다 int 로 변환
4. 부호 없는 정수형과 부호 있는 정수형이 섞여있는 경우: 부호 없는 정수형으로 변환된다.

```
int + unsigned int = unsigned int
long + int = long
float + int = float
short + byte = short
float + double = double
```
[예제](overflow.c)

예제를 실행해보면 4294967294 가 나온다.

이유는 (a + b) = usigned char 의 max 값
``
등등등 위의 설명을 읽음녀 이해가될 것이다.
## 실수 자료형의 이해
### 실수 연산의 어려움
[예제](obvious.cpp)

예제를 실행하보면 1.000000, 49 가 출력된다.
### 실수와 근사 값
우리가 일상적으로 다루는 정수들은 컴퓨터에서 모두 처리가 가능하다.

컴퓨터 메모리는 항상 유한하고, 이 모든 값들을 모두 정확하게 담기는 힘들다.

그래서 적절히 비슷한 값으로 만족해야 된다.

뿜빠이 할 때, 가위바위보로 조금 더 내는거랑 비슷하다고 보면 된다.

컴퓨터에서도 현실과의 타협이 이루어진다.

컴퓨터의 모든 실수 변수는 정확도가 제한된 근사 값을 저장한다.
#### IEEE 754
* 이진수로 실수를 표기
* 부동 소수점 표기
* 무한대, 비정규 수(subnormal number), NaN(Not a Number) 등의 특수한 값이 존재

실제로 IEEE 754 는 실수 연산에 관한 규정, 오버플로와 언더플로의 처리, 반올림에 관한 규정 등을 모두 포함하는 방대한 표준입니다.

이 모든것은 알아서 찾아보라
#### 실수의 이진법 표기
실수의 이진수 표기도 기본적으로 정수랑 똑같은 방식을 사용한다.

소수점 밑 i 번째 자리의 크기는 1 / 2^i 다.
#### 부동 소수점 표기
32비트의 공간을 사용해 실수를 이진법을 표기한다면?

정수부와 소수부에 어떻게 배분할지에 대해 고민해야 된다.

IEEE 754 를 포함한 대부분의 실수 표준에서는 소수점을 옮길 수 있다.

11.625 는 이진법으로 쓰면 1011.101 이 된다.

왼쪽으로 세 칸 옮기면 (소수점을) 1.011101 이 되고, 맨 앞에서부터 저장 공간이 허락하는 만큼 저장한다.

그런데 이진법에서는 소수점 위에 있을 수 있는 유일한 숫자는 1이다.

그래서 IEEE 754 에서는 1을 제외한 나머지를 저장하는 방식으로 1비트를 저장한다.

예를 들어 5비트만 저장할 수 있다면, 다음 5비트인 01110(1.011101 중 소수점 뒤 숫자들) 을 저장하게된다.

실수 변수는 다음과 같은 3가지의 정보를 저장한다.
1. 부호 비트(sign bit): 양수 음수 확인
2. 지수(exponent): 소수점을 몇 칸 옮겼나
3. 가수(mantissa): 소수점을 옮긴 실수의 최상위 X 비트

부호 비트는 1비트라고 치고, 지수와 가수에는 각각 몇 비트를 써야 될까?

용량이 정해져 있을 때, 지수와 가수가 갖는 비중을 어떻게 하냐에따라 정확도가 결정된다.

63 비트중 53 비트로 지수를 표현하고, 나머지 10 비트만 가수를 표현하는데 쓴다고 하면,

지수의 최대치와 최소치는 약 +-2^52 가 된다.

소수점을 약 4503조 자리나 움직일 수 있는 셈이다.

10비트로는 첫 위치의 1을 포함한다해도 최대 11비트 만을 표현할 수 있다.

그래서 정확도는 낮다.

**나중에 수학 공부를 더 하고 자세히 파보겠다.**