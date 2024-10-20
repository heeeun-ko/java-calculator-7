# java-calculator-precourse

## 문자열 덧셈 계산기

문자열 덧셈 계산기는 주어진 문자열에서 숫자를 추출하여 덧셈을 수행하는 프로그램입니다.

## 기능 목록

1. 빈 문자열을 입력할 경우 0을 반환한다.
2. 쉼표(,) 또는 콜론(:)을 구분자로 사용하는 문자열을 입력받아 각 숫자의 합을 반환한다.
    - 예시: `"1,2"` → 3, `"1,2:3"` → 6
3. 커스텀 구분자를 지정할 수 있다. 커스텀 구분자는 문자열 앞부분에 `"//"`와 `"\n"` 사이에 위치하는 문자를 사용한다.
    - 예시: `"//;\n1;2;3"` → 커스텀 구분자는 세미콜론(;)이며 결과값은 6
4. 음수가 포함된 숫자를 입력할 경우 `IllegalArgumentException`을 발생시키고, 에러 메시지와 함께 프로그램이 종료된다.
5. 잘못된 형식의 문자열이 입력될 경우 `IllegalArgumentException`을 발생시키고, 에러 메시지와 함께 프로그램이 종료된다.

## 사용 방법

1. 사용자는 문자열을 입력하면 해당 문자열의 구분자를 기준으로 숫자를 분리하고, 분리된 숫자의 합을 반환 받을 수 있습니다.
2. 커스텀 구분자가 포함된 문자열은 구분자가 `"//"`와 `"\n"`사이에 있어야 합니다.
    - 예시 입력: `"//;\n1;2;3"`
    - 예시 출력: `6`
3. 빈 문자열이 입력되면 결과는 `0`을 반환합니다.

## 예외 처리

- 음수가 포함된 문자열이 입력되면 `IllegalArgumentException`을 발생시키며, 에러 메시지를 출력합니다.
- 잘못된 형식의 입력에 대해 `IllegalArgumentException`을 발생시키고 애플리케이션이 종료됩니다.