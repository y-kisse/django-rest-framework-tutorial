# MEMO
## コンテナと必要パッケージの準備(1度しかしないもの)
- docker-compose.ymlとbackend/Dockerfileを作成
- `docker-compose run backend /bin/sh`でコンテナに入る。
  - `pip3 install django`, `pip3 install djangorestframework`を実行
  - `pip3 freeze > requirements.txt`でパッケージリストを保存
  - `exit`で戻ってくる。

## djnagoプロジェクトの作成  
imageを再度作成する。`docker-compose build`  
django projectを作成する。  
`docker-compose run backend django-admin startproject tutorial .`  
(カレントディレクトリに、tutorialという名称のプロジェクトを作成する。)  
