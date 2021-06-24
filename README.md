# Baukis2 - 顧客管理システム

## 説明

Baukis2は企業向けの顧客管理システム（学習用）です。

## 推奨されるシステム環境

* Docker
* Ubuntu 18.04
* Ruby 2.6.4
* Postgresql 11.2

## 注意事項

* 以下の手順では、一般ユーザーの権限でコマンドを実行してください。

## インストール手順

* このREADME.mdが存在するディレクトリでbin/bundleコマンドを実行してください。

## データベースのセットアップ

* このシステム専用のデータベースをPostgreSQL上に作成してください。
* データベースの接続パラメータに基づいてconfig/database.ymlを作成してください。
* bin/rails db:setupコマンドを実行してください。

## hostsファイルの設定

* ホストOSのhostsファイルに次の1行を追加してください。（要root権限）。hostsファイルは、Max OSXの場合は/private/etc/hostsフォルダに、Windowsの場合はC:/Windows/system32/driversフォルダにあります。

127.0.0.1 example.com baukis2.example.com

## システムの起動と終了

* bin/rails sコマンドを実行するとシステムが起動します。
* Ctrl-Cを入力するとシステムが終了します。

## システムの利用

* ブラウザで以下のURLにアクセスしてください：
  * http://baukis2.example.com:3000 -- 職員向けサイト
  * http://baukis2.example.com:3000/admin -- 管理者向けサイト
  * http://example.com:3000/mypage -- 顧客向けサイト