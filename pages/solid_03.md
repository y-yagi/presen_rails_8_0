# Solid Cable

* Pub/Subがサポートしていない環境でどう対応しているかというと、メッセージをテーブルに保存し、そのテーブルを専用のスレッドでポーリングしている
  * 更新があったら、メッセージ送信
* Rails 8.0で新規アプリケーションを作成した場合、そのテーブルを作成するschemaファイルの追加や、デフォルトでSolid Cableを使用するようAction Cableの設定がされているようになっている
* その他詳細は、[Solid Cableについてまなぼう](https://y-yagi-presen-solid-cable.vercel.app/)にまとめていますので、ご興味がある方はどうぞ
