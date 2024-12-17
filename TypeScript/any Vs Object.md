# any Vs Object
any 타입과 Object 타입은 모두 어떤 값이든 할당이 가능하다는 특징을 가지고 있습니다.
하지만 다음과 같은 차이점이 존재합니다.


```javascript
let notSure: any = 4;
notSure.ifItExists();
notSure.toFixed();

let prettySure: Object = 4;
prettySure.toFixed();
```
위 코드를 실행하면 어떻게 될까요?

![image](https://github.com/user-attachments/assets/7fd6ee40-72b7-441f-bddf-83e44adee683)

네 바로 위처럼 런타임 에러가 발생합니다.

![image](https://github.com/user-attachments/assets/cd4b65ce-9818-487d-bbb6-6ebc92c009bd)

하지만 Object 타입과 달리 Any 타입은 컴파일 시점에 에러를 잡아주지 못하는 것을 확인할 수 있습니다.
Object 타입 관련 코드만 남겨볼까요?

```javascript
// let notSure: any = 4;
// notSure.ifItExists();
// notSure.toFixed();

let prettySure: Object = 4;
prettySure.toFixed();
```

![image](https://github.com/user-attachments/assets/d202f9e9-e10f-4b23-983b-3527da9b6c67)

이처럼 Object 타입 관련 코드만 남겨놓으니, 실행해도 값이 안나오고 있습니다.
하지만 컴파일 시점에 에러를 잡아주기에 문제가 없다는 것을 알 수 있습니다.

### 요약
- 공통점
  - 어떤 값이든 넣고싶을 때 사용할 수 있습니다.
- 차이점
  - any : 컴파일러가 아예 잡기를 원하지 않을 때 사용
  - Object : 정의한 값과 관련된 동작이 아닐경우 컴파일 시점에 에러를 미리 잡아내고 싶을 때 사용

