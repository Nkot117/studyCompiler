# tsconfig.json を作成してコンパイルを実行する

- tsconfig.json を作成する<br>
  コマンド：tsc --init

- tsc コマンドでコンパイルを実行する

# tsconfig.json の設定を編集する

## コンパイルを実行するファイルを限定する

- exclude<br>
  コンパイル対象外のファイルパスを記載する。
- include<br>
  コンパイル対象のファイルパスを記載する。
- files<br>
  コンパイル対象のファイルパスを記載する。\*(ワイルドカード)は使えない。
- target<br>
  コンパイルする js のバージョン。デフォルトでは es3。
- lib<br>
  typescript が用意している型定義情報。デフォルトでは target に合わせた情報が設定される。
- allowJs<br>
  js ファイルをコンパイル対象に含めるか。
- checkJs<br>
  js ファイルのコンパイル時にチェックを行う。allowJs と一緒に使う。
- jsx<br>
  react の時に使う。
- declaration<br>
- declarationMap<br>
  型定義ファイル(.d.ts)を作成する。
- sourceMap<br>
  ブラウザで ts ファイルを確認できるようにする。
- outDir<br>
  js の出力先。
- rootDir<br>
  ts が格納されれいるフォルダの最長の親パスを指定する。
- removeComments<br>
  コメントを削除するか。
- noEmit<br>
  何も出力しない。型チェックのみ行う。
- downlevelIteration<br>
  target が es3 or es5 の時に使用するもの。es6 から追加されたイテレーション系の記法を、より正確に es3 or es5 にコンパイするするときに使う。
- noEmitOnError<br>
  エラーが起こったら js を出力しない。
- noImplicitAny<br>
  暗黙的な any を使用していないかチェックする。
- strictNullChecks<br>
  値が null になるようなプロパティを使用していないかチェックする。
- noUnusedLocals<br>
  使用されていないローカル変数がないかチェックする。
