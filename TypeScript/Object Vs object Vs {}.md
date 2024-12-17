# Object Vs object Vs {}
타입스크립트의 객체의 세가지 타입이 존재하는데, 헷갈리기 쉬워 정리하고자 한다.

## Object
- Object 타입은 Javascript의 객체와 완전히 동일하다고 할 수 있다.
- 즉 toString(), hasOwnProperty() 등 내장 함수를 가지고 있다.
- primitive type, none-primitive 모두 할당될 수 있다.
- 단, null과 undefiend는 할당이 불가능 하다.

## {}
- Object와 유사하지만 비어있는 객체이다.
- 컴파일 시점에 Object와 다른 상태이지만, 런타임 시에 Object와 동일한 구조를 가지게 된다.

## object
- non-primitive type을 할당할 수 있다.
- primitive type은 할당할 수 없다.
