<br>

## 리눅스 명령어 공부

<br>

[![Linux](https://img.shields.io/badge/Linux-E5B400?logo=linux&logoColor=000000&labelColor=E5B400)](https://github.com/Dobby/rename)

---


+ top
+ ps
+ jobs
+ kill

---

<br>

## top

<br>

+ top 명령어는 현재 os의 상태를 나타내주는 명령어
+ 메모리 사용량, CPU 사용량 등을 나타낸다.
+ top를 실행하는 동안에 주기적인 업데이트로 실시간에 근접한 내용을 보여준다.

<br>

 <img src="https://github.com/chacharone/chacharone/blob/main/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202025-11-28%20112140.png" width="70%">

#### top

+ 제일 왼쪽 위에 있는 것이 현재 시간이다.
+ 시간 오른쪽에 있는 것은 os가 살아 있는 시간이다.
+ 그 옆이 현재 접속중인 유저 세션 수 이다.

<br>

#### task

+ 실행(Runnable) - CPU에 의해서 명령어가 실행중인 Process
+ 준비(Ready) - CPU의 명령어 실행을 기다리는 Process
+ 대기(Waiting) - I/O operation이 끝나기를 기다리는 Process
+ 종료(Terminated) - Ctrl + Z 등의 signal로 종료된 Process
+ Zombie - Process는 root Process로 부터 뿌리내린 자식 Process의 형식으로 트리구조를 형성한다. 이 때 부모가 먼저 종료된 다면 root process로 부터 닿을 수 없는 Process가 생긴다. 이를 zombie process라고 부른다.

<br>

#### cpu

+ us : 프로세스의 유저 영역에서의 CPU 사용률
+ sy : 프로세스의 커널 영역에서의 CPU 사용률
+ ni : 프로세스의 우선순위(priority) 설정에 사용하는 CPU 사용률
+ id : 사용하고 있지 않는 비율
+ wa : IO가 완료될때까지 기다리고 있는 CPU 비율
+ hi : 하드웨어 인터럽트에 사용되는 CPU 사용률
+ si : 소프트웨어 인터럽트에 사용되는 CPU 사용률
+ st : CPU를 VM에서 사용하여 대기하는 CPU 비율

---

<br>


## ps

<br>

```Linux
ps [옵션]
```

+ ps 명령어는 UNIX 계열 운영 체제에서 현재 실행 중인 프로세스 목록을 표시하는 명령어
+ 옵션을 사용하여 용도 목적에 맞게 출력하게 할 수 있다.

 <img src="https://github.com/chacharone/chacharone/blob/main/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202025-11-29%20201452.png" width="70%">

 + -e 옵션 : 모든 프로세스를 나열한다.
 + -f 옵션 : 전체 포맷을 사용하며, 각 프로세스에 대한 상세한 정보를 보여준다.

| -f 옵션 | 설명 |
|------|------|
| UID | 사용자 ID |
| PID | 프로세스 ID |
| PPID | 부모 프로세스 ID |
| C | 프로세서 사용량 |
| STIME | 시작 시간 |
| TTY | 터미널 타입 |
| TIME | 총 CPU 사용 시간 |
| CMD | 실행 명령어 |

---

<br>

## jobs

<br>

```Linux
jobs [옵션]
```

+ jobs 명령어는 현재 세션에서 실행 중이거나 중단된 작업 목록을 출력하는 명령어
+ 옵션 없이 사용하면 현재 활성화된 작업 목록이 표시된다.
+ 단 실행중인 작업이 없다면 아무것도 출력되지 않는다.

 <img src="https://github.com/chacharone/chacharone/blob/main/%EC%8A%A4%ED%81%AC%EB%A6%B0%EC%83%B7%202025-11-29%20204724.png" width="70%">

| 옵션 | 설명 |
|------|------|
| -l | 프로세스 ID와 함께 잡 목록을 출력 |
| -n | 마지막로 알림 이후 변경된 잡만 출력 |
| -p | 잡의 프로세스 ID만 출력 |
| -r | 실행 중인 잡만 출력 |
| -s | 중지된 잡만 출력 |

---

<br>

## kill

<br>

+ kill 명령어는 특정 프로세스나 프로세스 그룹에 시그널을 보내 프로세스를 종료하는 명령

```Linux
kill [옵션] <프로세스 ID(PID)>
```

| 옵션 | 설명 |
|------|------|
| -15 | 정상 종료 |
| -9  | 강제 종료 |


---

<br>

## 정리

<br>

| 명령어 | 설명 |
|------|------|
| top | 현재 os의 상태를 나타내주는 명령어 |
| ps | 현재 실행 중인 프로세스 목록을 표시하는 명령어 |
| jobs | 실행 중이거나 중단된 작업 목록을 출력하는 명령어 |
| kill | 프로세스를 종료하는 명령 |





  


