# 下記のDocker composeを元にして作られました

https://github.com/oiax/rails6-compose

# 中にあるrailsアプリケーションは下記を元にして作られました

https://github.com/kuroda/baukis2

## 必要なソフトウェア

* Docker 18 以上
* Git 2.7 以上

## はじめかた

```
% git clone https://github.com/mako4kamiya/rails-system.git
% cd rails-system
% docker-compose up -d
% docker-compose exec web bash
% cd app
% bin/rails db:setup
% bin/rails assets:precompile
% bin/rails s -e production -b 0.0.0.0
```

※ ログアウトするには `exit` コマンドを実行するか、`Ctrl-D` キーを入力してください。

## コンテナ群の停止

```
% docker-compose stop
```

## コンテナ群の破棄

```
% docker-compose down
```
