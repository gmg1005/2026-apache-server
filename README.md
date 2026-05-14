## 사용 환경
- Ubuntu
- Apache
- PHP
- MariaDB

## 우분투 서버 구축
1. sudo apt update      # 패키지 업데이트
2. sudo apt install apache2 -y      # 아파치 설치
3. ip a     # 서버 IP 확인
4. 주소창에 IP주소 입력

### 기본 위치
/var/www/html/(secure,nosecure)        # 아파치 서버 
/ubuntu-server      # github 위치

## PHP 설치
1. sudo apt install php libapache2-mod-php php-mysql -y     # PHP 설치
2. sudo systemctl restart apache2       # 아파치 재시작
### PHP 동작테스트
1) cd /var/www/html/( )     # 웹서버 폴더로 이동
2) sudo nano test.php       # 테스트파일 생성
3) <?php
    phpinfo();
    ?>         #내용 입력후 저장
4) 브라우저에서 http://서버ip/test.php      #확인해보기

## MariaDB 설치
1. sudo apt install mariadb-server          # Maria DB 설치
2. sudo systemctl status mariadb        # 실행 상태 확인
3. sudo mysql       # MariaDB 접속