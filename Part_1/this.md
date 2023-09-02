# About this
- 일반 함수 내에서 사용하면 **window**, **전역객체**를 가리킨다.  
_❗️ [Window(전역객체)에 대하여](https://velog.io/@ouneno/JS-%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8%EC%9D%98-%EC%A0%84%EC%97%AD%EA%B0%9D%EC%B2%B4-window)_
- 오브젝트 내의 함수에서 사용하면 함수를 동작시키는 **오브젝트**가 출력된다.

```js
var 유저가져오기 = {
  name : 'ouneno',
  함수 : function() {
    console.log('유저가져오기.함수() 실행완료')
  },
  this함수 : function() {
    console.log(this)
  }
}
```

#### 결과
- 유저가져오기.함수()를 실행시 console에 찍혀있는 '유저가져오기.함수() 실행완료'가 출력됨을 볼 수 있다.  
- 하지만 this를 가리키고 있는 유저가져오기.this함수()의 경우에는 유저가져오기에 대한 모든 정보가 출력된다.
