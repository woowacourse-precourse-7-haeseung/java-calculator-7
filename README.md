# java-calulator-precourse

## 구현할 Method

### 1. 구분자 확인 Method

**시그니처**
```java
char checkDelimiter(String input);
```

**입력**
- 구분자와 양수로 구성된 문자열

**출력**
- 구분자가 있는 경우: 구분자 반환
- 구분자가 없는 경우: `null` 반환

**로직**
1. 입력 string으로부터 구분자 탐색
2. 존재하면 반환
3. 없으면 `null` 반환


### 2. 숫자 분리 Method

**시그니처**
```java
List<String> splitByDelimiter(String input, List<char> delimiter);
```

**입력**
- 양수로 구성된 문자열
- 기본 구분자와 커스텀 구분자

**출력**
- 구분자를 바탕으로 split된 수의 String List

**로직**
1. 문자열을 구분자를 바탕으로 split
2. 분리된 문자열 list 반환


### 3. 숫자 (String → Integer) 변환 Method

**시그니처**
```java
List<int(Integer)> checkDelimiter(List<String> numStrings);
```

**입력**
- 양수로 구성된 문자열 리스트

**출력**
- 리스트 각각의 문자를 Integer로 변환하여 반환

**로직**
1. 입력 문자들을 수로 변환 및 반환


### 4. 최종계산 Method

**시그니처**
```java
int(Integer) calculate(List<int(Integer)> nums);
```

**입력**
- 양수 리스트

**출력**
- 리스트의 길이가 0이 아닌 경우: 숫자의 합 반환
- 리스트의 길이가 0인 경우: 0 반환

**로직**
1. 리스트의 숫자를 하나씩 방문하며 합 계산
2. 계산된 값 반환