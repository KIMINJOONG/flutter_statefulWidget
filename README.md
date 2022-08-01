# Widget 이론
- Widget은 모두 "불변"의 법칙을 갖고있다.
- 하지만 위젯의 값을 변경해야할 때가 있다.(색 변경 등)
- 변경이 필요하면 기존의 위젯을 삭제해버리고 완전 새로운 위젯으로 대체한다.

# StatelessWidget 라이프 사이클(life cycle)
- Constructor로 생성이 되고 생성이 되자마자 build 함수가 실행된다.
- 이전 Container 예제와 마찬가지로 변경이 필요하면 새로운 위젯을 만들어 버린다.
- 하나의 StatelessWidget은 라이프 사이클동안 단 한번만 build 함수를 실행한다.

# StatefulWidget 라이프 사이클
1. Constructor
2. createState
3. initState
4. didChangeDependencies
5. dirty
6. build
7. clean (didUpdateWidget or setState)
8. deactivate
9. dispose

# 파라미터가 바뀌었을때 생명주기
1. Constructor(createState 실행 x)
2. 기존 State 재활용
3. didUpdateWidget
4. dirty
5. build
6. clean

# setState 실행시 생명주기
1. setState
2. dirty
3. build
4. clean


