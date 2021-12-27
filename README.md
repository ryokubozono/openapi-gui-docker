# OPENAPI-GUI-DOCKER

fork from [swagger-all-in-one-docker-compose](https://github.com/elevennines-inc/swagger-all-in-one-docker-compose)

## 概要

- [stoplight](https://stoplight.io/studio/) をローカルにinstallする
- [swagger-ui](https://hub.docker.com/r/swaggerapi/swagger-ui): API定義書をUI表示する。
- [apisprout](https://github.com/danielgtaylor/apisprout): モックAPIサーバー。
- [nginx](https://hub.docker.com/_/nginx): nginx。APIサーバーへのproxyを設定する。

- 作成したファイルはローカルに保持して、git管理する。
- ローカルの swagger/hoge.json が読まれる。（設定を書き換えて yaml に変更可能）

- 複数ファイルに対応していない。

## 起動

```sh
$ docker network create swagger_link # 初回のみ実行
$ docker-compose up
```

## ブラウザにアクセス

http://localhost:8080

## TODO

- M1 macだと以下のエラーメッセージが出るが、起動はできている。

```sh
swagger-ui     | 2021/12/27 08:01:20 [emerg] 89#89: io_setup() failed (38: Function not implemented)
```
