# WebStorm

## Refactor

### Rename
* 매개변수와 지역변수의 이름이 마음에 안들어 변경하고싶을 경우 하나 하나 수정하기에는 귀찮고 오타가 발생할 확률도 크다
* 이 때 사용 하는 것이 Rename Refactor을 이용해서 이름을 효과적으로 변경할 수 있다.
* 객체의 프로퍼티의 경우 다른 곳에서 사용하는 곳 까지 자동으로 변경해준다
* 존나 좋다

### Change Signature
* 함수나 메서드의 파라메터를 안전하게 추가하거나 삭제한다.
* 함수에 파라메터를 추가할 경우 해당 함수를 호출하는 곳에서도 더미데이터 형식으로 값을 자동으로 넘겨주게 할 수있다.

### Safe Delete
* 삭제하려는 변수나 객체의 의존 관계를 파악하여 안전성을 검사한다.
* 특정 함수를 사용하지 않을 거같아 제거할 경우 다른 곳에서 이함수를 호출하는 코드가 있을시 에러가 발생하게 된다.
* `Safe Delete`를 사용할 경우 해당 함수가 호출하는 모든 코드를 쉽게 보여준다.
* 다른 곳에서 사용하고 있으면 경고해준다.

### Inline Local Variable

* 간단한 수식의 결과값을 가지는 임수변수가 있고, 그 임시변수가 다른 리팩토링을 하는데 방해가된다면 이 임시변수를 참조하는 부분을 모두 원래 수식으로 변경해라 -마틴 파울러-
* 