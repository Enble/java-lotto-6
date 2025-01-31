# 기능 목록
## 시나리오별 기능 목록
### 사용자 입력
* 아래의 모든 경우에 대해, 사용자가 올바른 입력을 하지 않은 경우 사용자 입력을 다시 받는다.
* 로또 구입 금액 입력
  - `int`가 아닌 경우 예외 반환
  - 1000원 단위가 아닌 경우 예외 반환
* 당첨 번호 입력
  - `int`가 아닌 경우 예외 반환
  - 번호 개수가 6개가 아닌 경우 예외 반환
  - 1~45 사이가 아닌 경우 예외 반환
  - 중복되는 경우 예외 반환
* 보너스 번호 입력
  - `int`가 아닌 경우 예외 반환
  - 1~45 사이가 아닌 경우 예외 반환
  - 당첨 번호와 중복되는 경우 예외 반환

### 로또 번호 생성
* n개의 로또 집합에 대해 아래와 같이 수행한다.
  - 중복되지 않는 6개의 로또 번호 생성
  - 로또 번호 정렬
* 로또 번호와 중복되지 않는 보너스 번호 1개 생성

### 결과 출력
* n개의 로또 번호 세트 출력
* 당첨 내역 출력
* 수익률 출력 - 둘째 자리에서 반올림

### 에러 문구 출력
* 예외 상황시 `[ERROR]`로 시작하는 에러 문구 출력

---
## 기타 기능 목록

### 사용자 입력 검증
* 검증에 필요한 클래스 생성
* 예외 에러 문구 enum 생성

### 사용자 입력 파싱
* 사용자 입력을 파싱하여 로또 번호 및 보너스 번호 추출

### 수익률 계산
* 수익률 정책 저장을 위한 enum 생성
* 수익률 계산을 위한 클래스 생성

### 출력 관련 기능
* 사용자에게 출력할 메시지를 담은 enum 생성
