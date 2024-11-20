# Chatting

## Terminal chat programs based on Linux, C

server에서 FILE I/O를 이용해서 "log.txt" 파일에 chatting log를 기록하는 기능만 추가했습니다  
예시 : (2024-11-21 01:23:30) [name] chat text

name은 client에서 argv로 받아서 sprint함수 이용하여 send할때 같이 전송하도록 구현했고  
server에서 client 정보를 구조체로 저장하는 기능은 아직 구현 안 했습니다

### usage guide
```c

  ./cser
  ./ccli name

```

### compile method
```c

  gcc -o ccli ccli.c -pthread
  gcc -o cser cser.c -pthread

```
