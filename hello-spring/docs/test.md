# 테스트 코드를 작성하기

1. Assertions 활용
- Assertions.assertEquals(member, result);
2. assertThat 활용
- assertThat(member).isEqualTo(result)

테스트는 작성한 코드의 순서대로 실행 X(순서가 보장되지 않는다.)

그래서 만일 비슷한 도메인을 테스트하는 코드일 경우 예기치 못한 에러가 나타날 수 있다.

ex) A라는 객체를 저장하고 존재하는지 테스트\
A라는 객체를 저장하는 테스트\
이 두 테스트에서 저장이라는 기능이 중첩되어 오류가 뜬다.

그래서 저장소 테스트일 경우 매 테스트마다 저장소를 초기화하는 기능이 필요하다.

