# step.3

今回はswarm関連の説明はしないので、そういうこともできるんだなぁくらいの理解でよいです

    # 何もないことを確認
    docker service ls

    # swarmクラスタの初期化とデプロイ
    docker swarm init
    docker stack deploy -c docker-compose.yml my-docker-practice
    
    # 確認
    docker service ls

そのあと以下でアクセス確認

http://localhost:38080/
http://localhost:48080/

確認が終わったら不要なクラスタを解体する

    docker stack rm my-docker-practice
    docker swarm leave --force