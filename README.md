# java-lotto-precourse

## 기능 목록

- [x] 로또 구입 금액 입력에 따라 발행할 로또 개수를 정한다.
  - [x] 로또 구입 금액을 입력 받는다.
  - [x] 예외처리: 1000원으로 나누어 떨어지지 않는 경우
  - [x] 예외처리: null 또는 빈 값인 경우
  - [x] 예외처리: 숫자가 아닌 경우
  - [x] 예외처리: 음수인 경우
  - [x] 구입 금액이 1000원으로 나누어 떨어지는 경우, 1000으로 나누어 로또 개수를 정한다.

- [x] 로또 개수만큼 로또를 발행한다.
  - [x] pickUniqueNumbersInRange()를 활용하여 1에서 45 사이의 중복되지 않은 정수 6개를 뽑는다.
  - [x] 발행한 로또(Lotto)들을 Lottos에 저장한다.

- [x] 당첨 번호를 입력 받아서 저장한다.
  - [ ] 예외처리: null 또는 빈 값인 경우
  - [ ] 예외처리: 쉼표(,)로 구분되지 않은 경우
  - [x] 예외처리: 숫자가 아닌 경우
  - [ ] 예외처리: 1~45 범위의 숫자가 아닌 경우

- [x] 보너스 번호를 입력 받아서 저장한다.
  - [x] 예외처리: null 또는 빈 값인 경우
  - [x] 예외처리: 숫자가 아닌 경우
  - [x] 예외처리: 1~45 범위의 숫자가 아닌 경우
  - [x] 예외처리: 당첨 번호 6개와 중복되는 경우

- [ ] 발행된 로또 번호와 당첨 번호를 비교하여 당첨 내역을 출력한다.
  - [x] 5등부터 1등 순서로 당첨 개수를 출력한다.
  - [x] 실행 결과 예시 형식에 맞게 출력한다.

- [ ] 수익률을 출력하고 로또 게임을 종료한다.
  - [x] 수익률을 계산한다.
  - [ ] 수익률은 소수점 둘째 자리에서 반올림한다.

- 사용자가 잘못된 값을 입력한 경우
  - [ ] `IllegalArgumentException`을 발생시킨다.
  - [x] "[ERROR]"로 시작하는 에러 메시지를 출력한다.
  - [ ] 예외가 발생한 부분부터 입력을 다시 받는다.

- 테스트 코드를 작성한다
  - [ ] 구입 금액 예외처리 테스트
  - [ ] 로또 발행 테스트
  - [ ] Lotto 클래스(발행된 로또) 유효성 테스트
  - [ ] 당첨 번호 및 보너스 번호 입력 테스트
  - [ ] 당첨 내역 및 수익률 출력 테스트