프로그램은 메모리에 적재되고 실행되기 직전부터가 프로그램, 이라고 부를 수 있음.

프로그래밍과 타이밍
* 랭귀지 코드 - 린트 타임
* 머신 랭귀지 - 컴파일 타임
* 파일
* 로드 (메모리에 적재되는 때)
* 런 - 런 타임
* (런타임에는 문제가 없지만 에러가 존재하는 것은 컨텍스트 에러)
* 터미네이트(실행이 종료되면 메모리에서 사라짐)

랭귀지가 존재하는 이유는 사람이 기계어를 바로 짤 수 없기 때문.
타이밍이 존재하는 이유는 에러의 발생을 미리 찾아낼 수 있게 하기 위함.

스크립트 언어의 프로그램과 타이밍
* 랭귀지 코드 - 린트 타임
* 파일
* 로드
* 머신 랭귀지 (자바스크립트는 오토컴파일러임. 호출되지 않은 부분은 제외하고 부분적으로만 컴파일될 수 있음.)
* 런 - 런 타임
* 터미네이트

타입스크립트처럼 컴파일타임을 주는 보완책도 나옴.

자바스크립트는 런타임 밖에 없으므로
런타임의 기저가 되는 함수, 클래스
그리고 그것들 활용한 함수, 클래스가 있다면
각각의 기저의 정의 타임 (스태틱 타임, 런타임)
활용 함수, 클래스의 정의 타임에 따라 스태틱/런타임이 존재하게 됨
그 각각의 타임을 나누어서 복잡성을 낮추는 방법으로 격리를 사용

---

랙시컬 그래머
* control character 제어문자
* white space 공백문자
* line terminators 개행문자
* comments 주석
* keyword 예약어 (특정 기능을 수행하는 단어)
* literals 리터럴 (값을 나타내는 최소한의 표현, 더이상 쪼갤 수 없는 단위)

자바스크립트 엔진이 텍스트를 만나면 텍스트를 이렇게 나누어서 보게 됨


---

statements 문
자바스크립트 엔진이 어떻게 실행하면 좋은지에 대한 힌트. 값이 되지 않음. 힌트만 주고 메모리에 남지 않음. (값이 될 식과 문은 언어를 만드는 사람에 의해 정의됨)
* 공문(실수를 방지하기 위함), 식문(하나의 식은 하나의 문임. e.g. 3+5; 자바스크립트에서 가능한 문), 제어문, 선언문(식별자를 선언) 
* 단문, 중문(혹은 복문, 복수개의 문장을 하나의 문장으로 취급. 중괄호로 묶임)

expression 식 (하나의 값이 될 수 있는 식)
* 값식, 연산식(연산된 값), 호출식(함수의 리턴값)

identifier 식별자
값은 저장하지 않으면 즉시 메모리에서 휘발됨
* 기본형(값이 복사됨), 참조형(참조가 복사됨)
* 변수, 상수(변화 가능성을 제거함으로써 복잡성을 낮출 수 있음)

복잡성을 낮추고 수정 가능성을 확보해야함
