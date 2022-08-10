# 概要
これを使って、毎回使いまわせます
参考文献
https://zenn.dev/hibriiiiidge/books/49ee4063b10cec1df1a2/viewer/dc751838fa3715f814dd

# 使い方

## 1 アプリ作成
$ docker-compose run backend rails new . --api --force --database=mysql --skip-bundle

## 2 image作成
sudo docker-compose build

## 3 コンテナを立ち上げる
sudo docker-compose up