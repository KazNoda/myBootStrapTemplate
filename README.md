myBootStrapTemplate
===================

簡単なBootStrapのテンプレートです。

【テーブルのコンテンツ箇所のスクロールの位置】

・そのそもGoogleカレンダーと現在同じ仕組みでスクロールを作成している。
  Googleカレンダーはコンテンツが画面幅に収まる為スクロールは右に出ているが

プラグイン「jScrollPane」で解決できるか？
http://www.eupholab.net/post/55878847106
http://manos.malihu.gr/repository/custom-scrollbar/demo/examples/rtl_direction_demo.html

http://n.blueblack.net/articles/2012-09-17_01_bootstrap_jk_smooth_scroll/

[検索キーワード: bootstrap table fixed]
http://stackoverflow.com/questions/21168521/scrollable-table-with-fixed-header-in-bootstrap
http://stackoverflow.com/questions/11483378/twitter-bootstrap-scrollable-table-rows-and-fixed-header
↑★これがいいかも！

https://gist.github.com/i-scorpion/2948136

※テーブルの幅を同じにするのなら、スクロールしたら途中でコピーされたヘッダー箇所が出て来る方法でもいいかな。。


【検索】

1. ページネーション機能
- 現在選択されているページ番号によって見せる情報を変更
  - 現在選択されている番号をAjax処理前に取得し、request情報に追加すれば動作する。
- 表示する件数はデフォルトで「200件」で固定

2. ソート機能
- Handlebarsのテンプレートを「ヘッダ」箇所と「コンテンツ箇所で分ける」
  （初期表示時にはヘッダーとコンテンツをHandlebarsから出力するが、
   ソート時は「コンテンツ」箇所のみの変更にする。

     各列（カラム）の順はdata-order属性に保存するようにする。（sessionStorage）に変更で

きるようにデータの「設定箇所」と「取得箇所」のInterfaceは同じものを使用する。

   属性の値が何も入っていない時は、デフォルトを「昇順」にして表示する。

3. 動的に列を変更

  - 動的に列を変更しても問題ないようにする。
- 列を追加・削除時にはdata-is-show-column属性にtrueまたはfalseを設定する。（デフォル

トはfalse）※これもセッションで管理できるようにする。
- Ajaxで画面情報を再取得した場合も、取得前と同じ列が出るようにする。



【WF更新】

・送信するJSONの構造が変わるのでAPI仕様書を変更

changeWkStatus : {
     approval : [1,2,3,4,5],
        remove   : [6,7,8,9,10]
}

・チェックした行をサーバに送る。（オーダーIDの配列とステータス）
・設計書を読み、WF共通ロジックを作成する。



【CSVアップロード（WFの一括更新）】

・CSV読み取り時の処理は以下の通り。
①予め取得する列の名を配列形式で決めておく。
②読み込んだCSV文字列を改行コード(\n\r)でsplitした配列に入れ、
最初の一行目文字列を「,」でsplitして、①で設定したカラム名が「何列目」に存在するかを変数に保存

③2行目移行をfor文で回して、取得したカラム名を②で取得した変数を基に取得。
④最終的には上記のようなJSON形式ができる。


・JS側でCSVを解析し、WF毎にオーダーIDの配列が入ったJSONをサーバに送信する。
