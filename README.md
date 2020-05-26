# vueの入門者のためのシンプルなリポジトリ

Vue CLIで作成したデフォルトプリセットをちょっといじったプロジェクトです。  
フォークしたりクローンしたりして使ってください。

ブランチを切り替えることでいくつかのサンプルコードが入っているようにするつもりです。

現在のブランチリスト
- master：現在最新のsample
- sample1/data_and_mastash：dataとマスタッシュ展開2個
- sample2/v-model_and_data：v-modelによるデータバインドの使い方
- sample3/methods_and_eventCall：メソッドの作成とイベント（クリック）からの呼び出し
- sample4/increment_counter：メソッドから変数の操作とメソッドに引数を使う


## プロジェクトのセットアップ
リポジトリをチェックアウトして
```.bash
#初回のみ
npm install 
```

### 開発するとき
```
# なんかおかしくなったらCmd(Ctrl)+Cして止めてもう一回
npm run serve
#   App running at:
#  - Local:   http://localhost:8080/ 
#  - Network: http://192.168.11.8:8080/
# ↑みたいなメッセージが表示されるので、表示された Localのほうをブラウザで開く


```

### 最初に見るコード
src/App.vue を好きなエディタで開いてください。

### プロダクションビルドするとき
```
npm run build
```

### ライセンス
MIT
