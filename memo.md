* [Ruby on Rails — Rails 8\.0: No PaaS Required](https://rubyonrails.org/2024/11/7/rails-8-no-paas-required)
* [ONCE — Writebook](https://once.com/writebook)
* Enter Kamal 2 + Thruster
  * Kamalは元々MRSKでしたね
  * [Kamal: hot deployment tool to watch—or a total game changer?—Martian Chronicles, Evil Martians’ team blog](https://evilmartians.com/chronicles/mrsk-hot-deployment-tool-or-total-game-changer#who-will-benefit-the-most-from-kamal)
  * [Replace Traefik with kamal-proxy](https://github.com/basecamp/kamal/pull/940)
  * [Kamal Handbook: The missing manual](https://kamalmanual.com/handbook/)
  * [Why we're leaving the cloud](https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0)
* A Solid Reduction of Dependencies
* Getting SQLite ready for production
  * https://www.youtube.com/watch?v=wFUy120Fts8&t=0s
  * ↑の資料 [Supercharge the One Person Framework with SQLite \| Fractaled Mind](https://fractaledmind.github.io/2024/10/16/sqlite-supercharges-rails/)
    * [How \(and why\) to run SQLite in production \| Fractaled Mind](https://fractaledmind.github.io/2023/12/23/rubyconftw/)
* Replacing Sprockets with Propshaft
  * [ONCE \#1 is entirely \#nobuild for the front\-end](https://world.hey.com/dhh/once-1-is-entirely-nobuild-for-the-front-end-ce56f6d7)
* Generating the authentication basics
  * テーブルは2つusersとsessions
  * ログイン、ログアウト、パスワードリセット
  * cookieにはsession idを設定
  * サインアップフローは無し
    * これは通常アプリケーション毎に違う可能性がある為、とのこと
  * ログイン処理にはrate_limitが指定されている
＊ その他メモ
  * [37signals Dev — De\-cloud and de\-k8s — bringing our apps back home](https://dev.37signals.com/bringing-our-apps-back-home/)