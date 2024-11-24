# Chatting

## Terminal chat programs based on Linux, C

server에서 FILE I/O를 이용해서 "log.txt" 파일에 chatting log를 기록하는 기능만 추가했습니다  
예시 : (2024-11-21 01:23:30) [name] chat text

name은 client에서 argv로 받아서 sprint함수 이용하여 send할때 같이 전송하도록 구현했고  
server에서 client 정보를 구조체로 저장하는 기능은 아직 구현 안 했습니다  

+ !search, !showall, !quit, !help 명령어 구현하였습니다. // 2024-11-24

!help, !showall   

![team_2_help_showall](https://github.com/user-attachments/assets/666ace33-ae54-4f5a-b678-9b7aef8295a0)  

!search, !quit

![team_2_search_quit](https://github.com/user-attachments/assets/bc176055-907a-45fe-8faa-5d042dd90c8b)  

log.txt    

![team_2_log txt](https://github.com/user-attachments/assets/0f67b98e-6b58-476e-b7fd-18badef64f4f)


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
