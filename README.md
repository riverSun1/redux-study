# redux-study
* state의 값이 바뀔때마다. dispatch를 할때마다 red함수를 호출하게 하려면
subscribe에 render를 등록하면 된다.
=>store.subscribe(red);

* redux를 사용하지 않은 코드는 서로간의 강하게 의존을 하고있다.
해당 컴포넌트는 자신의 일에만 집중하고
다른 건 신경쓰지 않아도된다.
다른것과 얽혀있지 않다.

* state는 복제해서 쓰는 것이므로 원본을 수정하면 안된다.

* action에 대해서 그에 따른 상태가 보고 싶으면 
여기저기 console.log를 쓴다.

* redux는 관리해야하는 상태들은 모두 하나의 store에 보관되어있다.
redux는 단 하나의 store를 유지한다.
그리고 그 store는 reducer라는 것을 통해서 가공되기 때문에 
application의 상태가 궁금하면 reducer를 이용하면 된다.
=> console.log(action.type, action, state, newState)
