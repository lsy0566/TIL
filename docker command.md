- 
- 

   1 docker ps
   2 docker stop 79344408a683
   3 docker stop 7e5e6f7b8181
   4 docker ps
   5 clear
   6 docker ps -a
   7 docker container rm 52c0da766708
   8 docker container rm 87aa8d393291
   9 docker container rm 61ba42091f03
  10 docker container rm c9c969ef5015
  11 docker container prune
  12 docker container prune
  13 docker ps -a
  14 docker image ls
  15 docker run -d -p 8080 gihyodocker/echo:latest
  16 docker run -d -p 8080 gihyodocker/echo:latest
  17 docker ps
  18 clear
  19 docker ps
  20 docker rm c42c189eae8b  dec5eacc39d0
  21 docker stop c42c189eae8b  dec5eacc39d0
  22 docker rm c42c189eae8b  dec5eacc39d0
  23 docker run --name myweb1 -d -p 8080 gihyodocker/echo:latest
  24 docker ps
  25 docker run --name myweb1 -d -p 8080 gihyodocker/echo:latest
  26 clear
  27 docker stop myweb1
  28 docker rm myweb1
  29 clear
  30 docker run --name myweb1 -d -p 8080 gihyodocker/echo:latest
  31 docker run --name myweb2 -d -p 8080 gihyodocker/echo:latest
  32 docker run --name myweb3 -d -p 8080 gihyodocker/echo:latest
  33 docker stop my
  34 docker ps -q
  35 docker container ls
  36 odcker ls
  37 docker ls
  38 docker stop $(docker ps -q)
  39 docker rm $(docker ps -q)
  40 docker rm $(docker ps -qa)
  41 docker ps -qa
  42 docker ps -a



- 포트번호 반드시 명시
- 개발 
  - package.json
  - index.json
- node_js 설치
- npm install
  - node_js 설치 안하면 불가능
- npm start
  - node index.js





1. Nodejs 설치
2. 개발
   1. package.json
   2. index\.js
3. npm install
4. npm start



1. From -> Node 사용가능 한 이미지

2. RUN -> NPM INSTALL 실행

3. CMD -> NPM START



### Docker 주요 명령어

- -t

  - 태그 명렁어

  docker build -t edowon0623/simpleweb:latest .

- image ls -> images

- imge pull, push

- image rm -> rmi

- container ls -> ps

- ps -a (Stopped)

  - 멈춘 것 포함해서 보여준다

- container stop

- container rm

- docker rmi -f
  
  - 없애려는 것에 container까지 없애는 명령어
- exec -it
  - execution -input -tty(콘솔 터미널)
  - 커맨드를 뒤에 전달할 수 있음
  - 작동중인 것만 가능
- WORKDIR (directory)
  
  - ()에 복사하기
- COPY (1)(2)
  
  - 1을 2에 있는 디렉토리에 복사
- --no-cashe

- --name --rm
  
- 중지시 제거까지 가능
  
- system prune
  
  - 쓰지 않는 프로그램 삭제



- none
  - 이미지 스탑 및 삭제



docker run -d -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=true --name mysql mysql:5.7











docker exec -it hungry_turing hostname sh => 안됨





ls

ls /home

cd /home/node

- 명령어
  ps, stop, rm, images, rmi, pull, logs, exec, system prune -a

