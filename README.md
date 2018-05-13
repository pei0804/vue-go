# vue go

勉強メモ

# npm

```console
$ npm init
```

対話プロンプトでパッケージの定義っぽいのが出来た

```javascript
{
  "name": "vue-go",
  "version": "1.0.0",
  "description": "勉強メモ",
  "main": "index.js",
  "dependencies": {},
  "devDependencies": {
    "vue-loader": "^15.0.10",
    "webpack": "^4.8.3"
  },
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/pei0804/vue-go.git"
  },
  "author": "",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/pei0804/vue-go/issues"
  },
  "homepage": "https://github.com/pei0804/vue-go#readme"
}
```

## install

```console
# --save-dev 開発用の依存関係をpackage.jsonに登録する
$ npm install webpack vue-loader  --save-dev
# --save 実行に必要なライブラリをpackage.jsonに登録する
$ npm install vue --save
# グローバルにwebpackコマンドをインストールする
npm install webpack -g 
```

以下のような感じで入った。

``` javascript
  "dependencies": {
    "vue": "^2.5.16"
  },
  "devDependencies": {
    "vue-loader": "^15.0.10",
    "webpack": "^4.8.3"
  },
```

これで出来上がる`node_modules`はGoでいうところの`vendor`なので、リモートリポジトリにはaddしない。
今回は、使わないけど、デファクトな知識っぽいのでメモした。

