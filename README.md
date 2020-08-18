# Redux for Beginners React

Learning Vanilla-Redux and React-Redux

## Redux

-   상태 관리 라이브러리
-   컴포넌트들의 상태 관련 로직들을 다른 파일들로 분리시켜서 더욱 효율적으로 관리 할 수 있다.
-   컴포넌트끼리 상태를 공유하게 될 때 여러 컴포넌트를 거치지 않고도 손쉽게 상태 값을 전달 할 수 있다.
-   글로벌 상태 관리를 할 때 가장 효과적이다.

:exclamation: ps. 유일한 솔루션은 아니며, Context API를 통해서도 동일한 작업을 할 수 있다.

### Reducer

-   리듀서는 이전 상태와 동작을 받아 새 상태를 리턴한다.

-   리듀서는 반드시 순수 함수여야 한다. 이를테면 데이터베이스 호출이나 HTTP 호출 등 외부의 데이터 구조를 변형하는 호출은 허용되지 않는다.

-   리듀서는 항상 현재 상태를 '읽기 전용'으로 다룬다. 기존 상태를 변경하지는 않지만 새 상태를 리턴은 할 수 있다.

### Store

> 애플리케이션의 상태를 저장
>
> 리덕스에서는 한 애플리케이션 당 한개의 store를 만들게되며,
>
> 스토어 안에는 현재의 앱 상태와 리듀서가 들어가있고, 추가적으로 몇가지 내장 함수들이 있다.

### createStore

> store를 생성하기 위한 함수

```
import { createStore } from "redux";
```
