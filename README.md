# OPENAPI-GUI-DOCKER

fork from [swagger-all-in-one-docker-compose](https://github.com/elevennines-inc/swagger-all-in-one-docker-compose)

## 概要

- openapi-gui: ブラウザのGUIベースでAPI定義書を作成する。
- swagger-ui: API定義書をUI表示する。
- swagger-api: モックAPIサーバー。
- swagger-nginx: nginx。APIサーバーへのproxyを設定する。

- 作成したファイルはローカルに保持して、git管理する。
- ローカルの swagger/openapi.json が読まれる。（設定を書き換えて yaml に変更可能）


## 起動

```sh
$ docker network create swagger_link
$ docker-compose up
```

## dockerに入る

```
$ docker container exec -it openapi-gui sh
```

## ブラウザにアクセス

http://localhost:8080

