## ✔ 파이썬 장점, 단점

**장점**
- 쉽고 간결하다. 그래서 빠른 개발이 가능하다. 빠른 개발은 빠른 배포로 이어져 시장의 피드백을 받을 수 있다.
- 오픈소스 언어이므로 많은 모듈등이 존재한다.

**단점**
- 인터프리터 언어이기 때문에 속도가 느리다.

## ✔ 동적, 정적 타입 언어
- 동적 타입 언어는 type을 지정 해주지 않아도 된다.
- 정적 타입 언어는 변수를 선언할 때 꼭 타입을 지정해줘야 함
- Python

## ✔ 컴파일러(compiler) vs 인터프리터(interpreter)
먼저 어셈블리어란 기계어와 일대일 대응이 되는 컴퓨터 프로그래밍의 low level language이다.
**컴퓨터 구조에 따라 사용하는 기계어가 달라지며, 따라서 기계어에 대응되어 만들어지는 어셈블리어도 각각 다르게 된다.**
초기 컴퓨터 프로그램들은 모두 어셈블리어로 작성했는데, 새로운 아키텍쳐가 적용된 CPU가 나올때마다 프로그램을 새로 나온 CPU에
맞는 어셈블리어로 다시 작성해야 했다. 그래서 통일된 언어체계인 hign level language가 나왔는데 컴퓨터는 high level language로
작성한 코드를 바로 인식하지 못해서 이를 번역해줄 과정이 필요했고 이것이 **컴파일**이다. (번역에는 컴파일러 방식과 인터프리터 방식이 있다.)

**컴파일러**
- 전체 파일을 스캔하여 한꺼번에 번역한다
- 초기 스캔시간이 오래 걸리지만, 한번 실행 파일이 만들어지고 나면 빠르다.
- 기계어 번역과정에서 더 많은 메모리를 사용한다.(Object 파일 생성, 링킹 작업 추가로 필요)
- 전체 코드를 스캔하는 과정에서 모든 오류를 한꺼번에 출력해주기 때문에 실행 전에 오류를 알 수 있음
- 대표적인 언어로 C, C++, JAVA 등이 있다.  

**인터프리터**
- 프로그램 실행 시 한 번에 한 문장씩 번역한다.
- 한 번에 한 문장씩 번역 후 실행 시키기 때문에 실행 시간이 느리다.
- 컴파일러와 같은 오브젝트 코드 생성과정이 없기 때문에 메모리 효율이 좋다
- 프로그램을 실행시키고 나서 오류를 발견하면 바로 실행을 중지 시킨다. 실행 후에 오류를 알 수 있음
- 대표적인 언어로 Python, Ruby, Javascript 등이 있다.


## ✔ 리스트, 튜플?

**공통점**
- Python 기본 데이터 타입이 **순서대로**들어가 있는 데이터 구조 

**차이점**
- 리스트는 원소를 수정할 수 있는 mutable 객체이고, 튜플은 immutable 객체이다.


## ✔ 셋, 딕셔너리
- 셋은 기본 데이터 타입이 **순서가 없이**들어가 있는 데이터 구조이다.
- 셋은 원소의 중복을 허용하지 않는다
- 딕셔너리는 키와 값의 쌍으로 이루어진 원소를 가진 데이터 구조이다.

## ✔ 객체란?
- '속성'과 '행동'으로 이루어진 것
- Example : 자동차는 바퀴 4개, 색깔, 의자, 핸들 등의 속성과 전진, 후진 등의 행동을 가진 객체
- 파이썬에서 속성은 변수로, 행동은 함수로 나타낸다.

## ✔ 객체 지향 프로그래밍이란?
- 프로그램을 여러 개의 독립된 **객체**들과 그 객체들 간의 상호작용으로 파악하는 프로그래밍 접근법
- 프로그램을 **객체**들 간의 소통으로 바라보는 것
**객체를 만드는 법**  
1. 프로그램에 어떤 객체들이 필요할 지 정한다.  
2. 객체들의 속성과 행동을 정한다.  
3. 객체들이 서로 어떻게 소통할 지 정한다.  

## ✔ __init__, __str__
언더바 두개에 쌓여있는 메서드를 magic method, 특수 메소드라고 부른다.  
magic method는 특정 상황에서 자동으로 호출되는 메소드다.  
- __init__ 메서드는 클래스 생성시 자동으로 호출된다.
- __str__ 메서드는 인스턴스를 프린트 했을 때 원하는 값이 나오게 한다.

## ✔ 절자 지향 프로그래밍 vs 객체 지향 프로그래밍
- 절차 지향 프로그래밍은 프로그램에 필요한 데이터를 관련있는 함수와 묶어서 관리하기 힘들다. 그러나  
객체 지향 프로그래밍은은 서로 관련있는 데이터와 함수를 객체로 묶어서 사용할 수 있다. by Class
- 절차 지향 프로그래밍은 프로그램을 단지 명령어들을 순서대로 실행하는 것, 객체 지향 프로그래믕은 프로그램을  
객체 간의 소통으로 본다. 즉 객체가 프로그램의 기본 단위가 되고, 이 객체 속을 들여다보면 서로 관련된 데이터(객체의 속성)와 동작(객체의 행동)이 모여있다. 그리고 프로그램을 이 객체들이 순서대로 소통하는 과정으로 간주
- 데이터와 동작의 연관성이 높고 이걸 객체라는 단위로 묶는 것이 낫겠다는 생각이 들면 객체 지향 프로그래밍이 좋음
- 보통 복잡한 프로그램일수록 객체 지향 프로그래밍이 나음

## ✔ 추상화?
- 특정 코드를 사용할 때 필수적인 정보를 제외한 세부사항을 가리는 것
- 커피 머신 내부 작동 원리를 몰라도 커피 머신을 쓸 수 있다.
- 변수에 값을 할당하는 것, 함수, 클래스를 사용하는 것 모두 추상화
- 예를 들어 list.append(값) 뒷다넹서 돌아가는 클래스 내부 로직을 몰라도 append를 사용할 수 있는 것처럼
- 추상화를 잘 하려면 이름을 잘 짓거나, 문서화(docstring)를 잘 해야 함

## ✔ 캡슐화?
- 객체의 일부 구현 내용에 대한 외부로부터의 **직접적인 액세스를 차단**하는 것
- 객체의 속성과 그것을 사용하는 행동을 하나로 묶는 것
- 변수나 메서드 이름 앞에 언더바 두개를 붙여준다.
- 캡슐화 된 변수의 값을 읽어주는 메서드는 getter, 할당 해 주는 메소드를 setter라고 한다.  

**네임 맹글링**
사실 언더바 두개를 붙인 변수나 메소드에 접근이 가능함.  앞에 '(언더바1개)클래스이름'을 덧 붙여서 이름을
새로 바꾼 녀석으로 접근이 가능함 이름을 새로운 형태로 변환하는 것을 네임 맹글링(name mangling)이라고 한다  
따라서 **외부에서 접근가능함 !! 사실 파이썬은 언어 차원에서 캡슐화를 지원하지 않음** 캡슐화 처럼
보이는데 완벽한 캡슐화는 아님. 그러나 다른 객체 지향 언어인 java에서는 **private**라는 키워드를 변수 이름 앞에 붙이면
외부로부터의 접근이 완벽히 차단된다. 

**진짜 캡슐화 약속**
- 변수나 메소드 앞에 **언더바 하나**를 붙인다.

## ✔ 상속(Inheritance)
- 두 클래스 사이에 부모-자식 관계를 설정하는 것
- 자동차는 벤츠의 부모이다. 벤츠는 자동차를 상속받는다
- 상속은 반복을 줄여준다

**overriding**
- 부모의 변수를 오버라이드 하려면 똑같은 변수명으로 오바리이드 하면 된다.
- super().언더바2개init언더바두개(똑같은 인자)로 상속을 명시할 수 있음 (이렇게 안해도 자동으로 상속은 됨)
