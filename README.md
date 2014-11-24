・検索画面で会社区分を取得して初期表示
・「ボタン」からアップロード

・検索画面の並べ替え
・権限に応じて画面パーツの出しわけ
・全検索すると落ちる。
・JUnitで自動テスト
・<th>をクリックしても#がつかないようにする。
・共通化
・ジェネリクスが使えないか再度確認
・必須チェックの必要性をもう一度見直す。
・検索一覧に表示させるリンクがクリックできない理由を確認

・メニュー画面パーツの表示・非表示の有無



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

1. 例外処理

if (typeof a !== 'number' || type b!== 'number') {
    throw {
        name : 'TypeError',
        message : 'add needs numbers'
    };
}

try {
   add("seven");
}catch (e) {
    document.write(e.name + ' : ' + e.message);
}

2. コード整理



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
最初の一行目文字列を「,」でsplitして、①で設定したカラム名が「何列目」に存在するかを

変数に保存
③2行目移行をfor文で回して、取得したカラム名を②で取得した変数を基に取得。
④最終的には上記のようなJSON形式ができる。


・JS側でCSVを解析し、WF毎にオーダーIDの配列が入ったJSONをサーバに送

信する。
