### 예시 코드
```ts
const data = "[{
	'a': 3
}]"
```

### 위 형식의 string을 array로 바꾸는 방법
```ts
const parsedData = JSON.parse(datareplaceAll("'", '"'))
```
- '을 "으로 바꾼 다음, JSON.parse를 사용한다.