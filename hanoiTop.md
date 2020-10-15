```js
function move(N,start,to){
  console.log(`${N}번 원반이 ${start}에서 ${to}로 이동`)
  }

function hanoi(N,start,to,via){
  if(N === 1){
    return move(1,start,to);
    }else{
      hanoi(N-1,start,via,to)
      move(N,start,to)
      hanoi(N-1,via,to,start)
      }
 }
 ```

```js
function hanoiCount(N){
  console.log(Math.pow(2,N) - 1)
  }
```
