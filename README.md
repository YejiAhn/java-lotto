# java-lotto
로또 미션 진행을 위한 저장소

## 1단계 - 기능적 요구사항
- [x] 구입금액 입력을 받아오는 기능 (View)
    - **예외**
      - [x] 숫자가 아닌 경우 
      - [x] 1000원이 되지 않는 경우
      - [x] 1000원의 배수가 아닐 경우
- [x] 구입금액으로 로또를 몇 개 구입했는지 알려주는 기능 
- [x] 갯수에 맞춰 로또를 자동으로 생성해주는 기능
    - [x] 1에서 45까지의 숫자 `enum` 생성
- [x] 지난 주 당첨번호 입력받기 (쉼표(, )로 구분)
    - **예외** 
      - [x] 숫자가 중복되는 경우
      - [x] 입력받은 숫자가 여섯 개가 아닌 경우
      - [x] 입력받은 숫자 중 0 이하 혹은 46 이상의 숫자가 포함된 경우
      - [x] 쉼표나 숫자 외의 입력값이 들어오는 경우
- [x] 보너스 볼 번호 입력받기
    - **예외**
      - [x] 숫자가 아닌 경우
      - [x] 당첨번호와 중복되는 경우
      - [x] 0 이하 46 이상의 숫자인 경우
- [x] 당첨 통계 내주는 기능
- [x] 수익률 계산해주는 기능

## 2단계 - 기능적 요구사항
- [x] 수동으로 구매할 로또 수를 받아오는 기능
    - **예외**
        - [x] 숫자가 아닌 경우
        - [x] 구입 금액을 넘어서는 수량일 경우
        - [x] 음수일 경우
- [x] 수동으로 구매할 로또 번호의 입력을 받아오는 기능 (당첨번호 입력 기능과 동일)
- [ ] 남는 금액으로 자동 로또를 생성하고 수동 로또와 합쳐 객체를 만드는 기능

## 1단계 - 비기능적 요구사항
- indent(인덴트, 들여쓰기) depth를 2단계에서 1단계로 줄여라.
    - depth의 경우 `if`문을 사용하는 경우 1단계의 depth가 증가한다. if문 안에 `while`문을 사용한다면 depth가 2단계가 된다.
- `else`를 사용하지 마라.
- 메소드의 크기가 최대 10라인을 넘지 않도록 구현한다.
    - 메소드가 한 가지 일만 하도록 최대한 작게 만들어라.
- 배열 대신 `ArrayList`를 사용한다.
    - `enum`을 적용해 프로그래밍을 구현한다.
    
## 2단계 - 비기능적 요구사항
- 예외가 발생하는 부분에 대해 자바 Exception을 적용해 예외처리한다.
- 사용자가 입력한 값에 대한 예외 처리를 철저히 한다.