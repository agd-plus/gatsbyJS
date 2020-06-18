<!-- AUTO-GENERATED-CONTENT:START (STARTER) -->
<p align="center">
  <a href="https://dstrikes.net/2018/11/03/30years_old_start_at_programming/">
    <img alt="Gatsby" src="https://dstrikes.net/wp-content/uploads/69632.jpg" width="180" />
  </a>
</p>
<h1 align="center">
  30代からのプログラミングGatsbyJSをいじってみた
</h1>
**追記**
日本語チュートリアルサイトを作りました！
これからGatsbyJSを学ぼうと考えてる方は是非、ご利用ください


[GatsbyJS日本語チュートリアル](https://npmja.com/)


プログラミング初心者がGatsbyJSのチュートリアルをやった際のレポジトリです。  
GatsbyJSの公式READMEを編集しながら書いていきます。

## 🚀 クイックスタート

1.  **Gatsbyインストール**

    下のコマンドを入力してGatsby-cliをインストール<br>
    事前にnode.jsをインストールしておく必要があります。

    ```shell
    # create a new Gatsby site using the default starter
    npm install -g gatsby-cli
    ```
    CLIインストールでエラーが連発される場合は以下

     ```shell
    # CLIがインストール出来くてもプロジェクトをインストール出来ます。　
    npx gatsby new gatsby-site https://github.com/gatsbyjs・gatsby-starter-default
    ```

    **ちなみにyarnでもGatsby-CLIがインストール出来る**

    ```shell
    # 先に新規フォルダを制作してフォルダの中で以下コマンドを実行する
    yarn add getsby-cli
    ```
2.  **GatsbyJS参考サイトや書籍**
  私がGatsbyJSを試すに当たって参考になったサイトや書籍を紹介します。
  * [Gatsby公式サイト(英語)](https://www.gatsbyjs.org/)
  * [ブログをGatsbyJS v2で実装したらめちゃくちゃ楽だった](https://www.ebiebievidence.com/posts/migrate-to-gatsby/)
  * [Gatsby.jsでサイト作成](https://blog.hokuma.net/frontend/gatsbyjs_site_generator/)
  * [基礎から始めるGatsbyJS入門](https://reffect.co.jp/react/gatsby-basic-tutorial-for-beginners)
  * [Webサイト高速化のための　静的サイトジェネレーター活用入門](https://amzn.to/2BmhG5v)
  * [Gatsbyでフォント関連のスタイルの設定をする](https://tech.glatchdesign.com/gatsby-typographyjs)[書籍]
  * [Gatsby で gatsby-theme-blog を使うときの tips](https://gotohayato.com/content/502/)
## GatsbyJSの構造

  ```shell
  ┏─ gatsby-browser.js
  ├─ gatsby-config.js
  ├─ gatsby-node.js
  ├─ package.json
  ├─ public
  ├─ node_modules
  ├─ src
  │   ├─ components
  │   ├─ pages
  │   └─ templates
  ```
### gatsby-config.js

  gatsbyサイトの設定全般情報を設定するファイルです。<br />
  メタデータや利用するプラグインの設定が行えます。

### gatsby-node.js

  Gatsby Node APIsとやり取りをするものらしいですが、まだ使った事がないので今後使った時に理解して解説します。

### gatsby-browser.js

  ブラウザでの表示時に実行される設定を書くらしいですが初期状態ではコメントアウトしかありませんので、こちらも今後なにか分かったら更新していきます。

### package.json

  gatsbyのインストールされたパッケージ情報一覧です。<br />
  gatsbyのシステムが利用するものなので普通は触らなくてOKです。

### public
  ```shell
  gatsby build
  gatsby develop
  gatsby serve
  ```
  上記コマンドでシステムを書き出したHTMLやCSSやJSファイルがここに生成されます。<br />
  静的サイトとしてアップするのも、このフォルダの中身だけです。

### node_modules

  インストールしたパッケージのファイルが格納されています。

## srcの役割

  src/配下のフォルダはサイト構成ファイルをまとめたものになります。<br />
  pagesはページファイル<br />
  templatesはレイアウトファイル<br />
  componentsはCSSやJSファイルを設置します。<br />

### src/components

  header.js / footer.js / image.js / layout.css / layout.js / seo.jsが格納されていますので、編集してサイトの大枠を作ります。

### src/pages

  ここにjsファイルを設置してページを作ります。
  ```shell
  gatsby build
  ```
  コマンドで生成されたファイルはpublicに格納されます。

### src/templates

  サイトの共通設定を格納するディレクトリ<br />
  こちらのサイトが詳しく解説してくれています。
  [Gatsby のファイル構成](https://suzukalight.com/2019-07-01-file-structure/)











end of markdown
