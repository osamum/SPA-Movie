# SPA-Movie

このプロジェクトは、Azure PaaS のデプロイから運用までを説明するハンズオン用のアプリケーションです。

このアプリケーションは、ハンズオン用の演習アプリケーションがホストする REST API を使用して動作する SPA (Single Page Application) です。

ページの生成はサーバーサイド ロジックに依存しないので API にさえアクセスできる Web サーバーであればどこでも動作します。

<br>

## 動作環境

HTTP をホストする Web サーバー上に配置し、index.html をブラウザーで開くことで動作します。

JavaScript フレームワーク、トランス スクリプトを使用していませんのでコンパイル、トランスパイルの必要はありません。  


<br>

## プロジェクトの入手と実行の準備

このリポジトリをクローンするか、ZIP ファイルをダウンロードしてください。

プロジェクト `js/site.js` の 2 行目にある MOVIEAPP_API を、ハンズオン用の演習アプリケーションがホストする REST API の URL に変更してください。

```js
// MovieApp APIのURL
const MOVIEAPP_API = 'ここに MovieApp-XYZ API の URL を入力してください';
```


## アプリケーションの実行
具体的な手順は以下の通りです。

1. Visual Studio Code を起動し、\[**ファイル**\] メニューから \[**フォルダーを開く**\] をクリックし、先ほどクローンしたプロジェクトのフォルダーを選択します

2. プロジェクト中のファイル `js/site.js` の 2 行目にある変数 **MOVIEAPP_API** の値を、ハンズオン用の演習アプリケーションがホストする REST API の URL に変更します

    ```JavaScript
    // MovieApp APIのURL
    const MOVIEAPP_API = 'ここに MovieApp-XYZ API の URL を入力してください';
    ```

    変更が完了したらキーボードの \[Ctrl\] + \[S\] キーを押してファイルを上書き保存します 

3. Visual Studio Code の画面右下にある \[**Go Live**\] ボタンをクリックします

    <img src="https://github.com/osamum/Azure-AppService-handson/raw/main/images/VisualStudioCode_launch_LiveServer.png" width="500px">

    しばらくすると HTTP でのホストが開始されますので、ホストされるポート番号を覚えておきます。(※既定では 5500 です)

4. ブラウザーが起動し、MovieApp SPA の UI が表示されます。