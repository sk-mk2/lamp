## LAMPでのサーバー勉強

sysv-rc-confでサービスの管理を管理簡単にできる
Dockerで構築しよう
### Docker
[docker get started](https://docs.docker.com/get-started)
動いてるコンテナをなくす: kill id 
イメージ作成: build
イメージの確認: image ls
コンテナ立ち上げ: docker run [OPTION] IMAGE [COMMAND] [ARG...]
コンテナ内で作業: docker exec -it コンテナ名 bash


### Apache
[あぱっちこうしきどきゅめんと](http://httpd.apache.org/docs/2.4/)
/etc/apache2に色々設定がある
apache2.confにいろいろな設定が書いてある
confは設定ファイル
modsはcgi使うとか、リクエスト振り分けとかする拡張機能の設定
sitesはバーチャルホストの設定

Webサーバ再起動: sudo systemctl apache2 restart 
コンフィグ反映: a2enconf ${設定ファイル}

### MariaDB
[MariaDB公式ドキュメント](https://mariadb.org/)

### PHP
[PHP公式ドキュメント](http://php.net/manual/ja/index.php)


## やりたいこと
リクエストの振り分け
大量のリクエストが来た時Nginxとの性能比較

