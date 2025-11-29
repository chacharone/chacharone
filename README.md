<br>

## 리눅스 명령어 공부

<br>

[![Linux](https://img.shields.io/badge/Linux-rename-E5B400?logo=linux&logoColor=000000&labelColor=E5B400)](https://github.com/Dobby/rename)

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

+ 제일 왼쪽 위에 있는 것이 현재 시간이다.
+ 시간 오른쪽에 있는 것은 os가 살아 있는 시간이다.
+ 그 옆이 현재 접속중인 유저 세션 수 이다.

---

<br>


## ps

<br>

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

+ jobs 명령어는 현재 세션에서 실행 중이거나 중단된 작업 목록을 출력하는 명령어
+ 옵션 없이 사용하면 현재 활성화된 작업 목록이 표시된다.
+ 단 실행중인 작업이 없다면 아무것도 출력되지 않는다.



  


