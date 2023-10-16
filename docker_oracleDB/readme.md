# Oracle XE 11g Docker Container

Oracle Express Edition 11g 데이터베이스를 실행하는 Docker 컨테이너를 구축하고 사용합니다. 이 컨테이너는 Oracle XE 11g 커뮤니티 버전을 기반으로 합니다. 

## 사용법

1. 먼저 Docker를 설치하십시오. [Docker 공식 웹사이트](https://www.docker.com/get-started)에서 다운로드 및 설치할 수 있습니다.

2. 이 프로젝트의 Dockerfile과 초기화 스크립트(init.ora)를 내려받으세요.

3. docker pull image:

   ```bash
   docker pull jaspeen/oracle-xe-11g
   ```
4. docker run container:

   ```bash
   docker run --name <컨테이너 이름> -d -p 8080:8080 -p 1521:1521 jaspeen/oracle-xe-11g
   ```
5. 컨테이너 실행 확인:

   ```bash
   docker ps # 실행 중인 컨테이너 확인
   ```
6. 컨테이너를 통한 OracleDB 접속:

   ```bash
   docker exec -it <컨테이너 이름> sqlplus 
   ```
7. 컨테이너를 통한 OracleDB 접속:

   ```bash
   SQL*Plus: Release 11.2.0.2.0 Production on Sun Oct 17 00:15:45 2023
   Copyright (c) 1982, 2011, Oracle. All rights reserved.
   Enter user-name:system
   Enter password:oracle
   Connected to:
   Oracle Database 11g Express Edition Release 11.2.0.2.0 - 64bit Production

   SQL>
   ```
