# ハンズオン
## ゴール
素のVueでTodoアプリ作れるようになろう
## 流れ
1. 準備
2. HelloHoge
3. イベントハンドリング
4. コンポーネント化
5. emit
6. Vuex
7. Router

## 1.準備
できればすましてきてほしい。。。
* node.jsのインストール
* vue開発環境の構築
* vue-cliのインストール

## 2.HelloHoge (sample-hoge)
双方向バインディング

## 3.イベントハンドリング (sample-button)
`v-on:イベント名`

## 4.コンポーネント化 (sample-button)
3のやつを2つに分ける。
やり方は2通り。(propsで引数として渡す or イベントの処理を渡す。)
* 入力コンポーネント
* ボタンコンポーネント

## 5.emit (sample-todo)
イベントを元のコンポーネントに伝える
ここまで出来たらTodo作ってみよう。
## 作ってみましょい
### Todo要件
* タスクを一覧で表示可能
* タスクの追加が可能
* タスクの名前でフィルタリング
* タスクの消化、未消化を切り替えられること
* タスクの削除ができること

## 6.vuex
action mutation state  の関係を学ぶ
* action  
APIの呼び出しとかする時はここ
* mutation  
stateに変更を加えるだけ
* state  
状態を保持するだけ

※状態を共通化するだけならstoreで十分  
※vuexを取り入れると型安全な世界が崩れる

## 7.Router
あまり難しくはない

## Build Setup
あまり難しくはない

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```
