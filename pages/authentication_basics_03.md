# Generating the authentication basics

* ログイン、ログアウト、パスワードリセットが実装されている
  * ログインしたらセッションテーブルにレコードが作成され、* cookieにはそのレコードのIDが指定されている
* サインアップフローは無し
  * これは通常アプリケーション毎に違う可能性がある為、とのこと
  * 当然アカウント削除も無し
* 実際に生成されるコードは[こちら](https://github.com/y-yagi/eightman/commit/d2e45b466c97196fb60df2daa160a742aceeb87b)