1. .env 에서 항목들 확인해서 설정

2. 최상위 폴더에 id_rsa, id_rsa.pub 복사

3. ./php/.env 에서 laravel 에서 사용할 env 설정

4. ./percona/setup.sql 에서 처음 생성될 database, user sql 설정

5. docker-compose 의 up으로 docker 실행
    예 ) docker-compose up -d --build

6. vscode 의 [Remote-Container: Open Folder In...] 기능을 이용해서 ./php/ 접근하면 User - newticle 로 소스코드 수정 가능

7. hosts 폴더에 임시 url 처리
    예 ) 192.168.0.1 58080 dev-main.newticle.com

8. newticle-php 에 들어가서 user - newticle 로 각각 디렉토리에서 명령어 입력
 dir-1 : /home/newticle/main
 dir-2 : /home/newticle/api

 - composer install
 - php artisan key:generate
 - php artisan migrate
