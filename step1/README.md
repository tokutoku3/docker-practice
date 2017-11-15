# step.1

apacheコンテナの起動とアクセス

    cd <docker-practice path>/step1
    docker build -t practice-step1 .
    docker run -dit -p 8080:80 --name my-practice-step1 practice-step1

上記コマンド実行後、下記にアクセス

http://localhost:8080/index.html