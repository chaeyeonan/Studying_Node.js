# Studying_Node.js

1. **전체 라이브러리 가져오기**

```jsx
const eachOfLimit = require('async');
```

만약 **`async`** 라이브러리의 모든 함수를 사용하고 싶다면, 전체 라이브러리를 가져온 후 특정 함수를 사용할 수 있다.

```jsx
// 함수 사용시
async.eachOfLimit(...);
```

1. **개별 함수 가져오기**

```jsx
const eachOfLimit = require('async/eachOfLimit');
```

하지만 특정 함수만 필요한 경우, 해당 함수를 직접 가져올 수 있다. 이 방법은 불필요한 메모리 사용을 줄이고 애플리케이션의 로딩 시간을 단축할 수 있다.

```jsx
// 함수 사용시
eachOfLimit(...);
```

## Collections 
### ~Limit 함수

- 기본 함수와 기능은 동일하나 비동기작업을 할 수 있는 항목의 개수가 제한적

### ~Series 함수

- 비동기 함수가 동시에 실행되지 않고 순차적으로 실행됨 (이전항목 끝나면 다음항목 실행)