## Remember

컴포저블은 기본적으로 상태가 없는 **Stateless**다. 즉, 시스템에서 언제든지 다시 구성하고 값이 재설정된다. 허나 특정 값이 바뀌지 않고 남아있어야 하는 상황이 생기기 마련이다.  

컴포즈에선 이러한 상황을 간단하게 방지할 수 있는 기능을 제공한다. 바로 `remember`다.

- `remember`를 사용하려면 함수를 전달해야 한다.
  `remember`는 보통 `mutableStateOf()` 함수와 많이 쓰인다. `mutableStateOf()` 함수는 `observable`을 반환한다.

```kotlin
var result by remember { mutableStateOf( /*any value*/ ) }
```

> 상태에 관한 더 자세한 사항은 [이 문서](https://github.com/boiledCompose/3_Tip-Calculator)에서 볼 수 있다.
