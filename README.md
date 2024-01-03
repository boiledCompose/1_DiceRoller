# DiceRoller
> 버튼을 누르면 주사위 면 중 하나를 보여주는 상호작용 주사위 굴리기 애플리케이션

### Modifier
1. fillMaxSize(): 이 메서드는 구성요소가 사용 가능한 공간을 채우도록 지정합니다
2. wrapContentSize(): 사용 가능한 공간이 최소한 내부에 있는 구성요소만큼 커야 한다고 지정합니다

- fillMaxSize()가 선언됐을 때, wrapContentSize()를 체인닝하여 내부 구성요소들을 정렬할 수 있습니다.

### Button
- Button의 내부에 Text나 Image와 같은 요소들을 집어넣을 수 있습니다.
- Button은 onClick이란 메서드를 포함해야 합니다.

### Remember
- 컴포저블은 기본적으로 스테이트리스(Stateless)입니다. 즉, 값을 보유하지 않고 시스템에서 언제든지 다시 구성할 수 있어 값이 재설정됩니다.
- 컴포즈를 사용하여 컴포저블에 스테이트를 부여할 수 있습니다. 구성 가능한 함수는 remember 컴포저블을 사용하여 메모리에 객체를 저장할 수 있습니다.
    <pre><code>
      var result by remember { mutableStateOf(1) }
    </code></pre>
