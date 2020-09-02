# mixture_app

環境構築はこちらからどうぞ
https://flutter.dev/docs

Flutter SDKはv1.20.2を選択してください

## How to build
macの人向け

AndroidstudioもしくはVScodeで作業します。
どちらでもいいけど、Androidstudioはコードフォーマットや自動補完がデフォルトで入ってるのでおすすめ.
(文法がわからんでもどうにかなったりする🐈)

iosのビルドにはXcodeのios Simulatorが必要です。
Androidのビルドには何も要らなかったはずです。
シュミレーターを起動後、ツールバーのRunアイコンもしくはDebugアイコンを押すとビルドされます。

今回しようするARkitはiosでしかビルドできないようです。
ARのテストをするときはUSBを実機に繋いでね

https://pub.dev/packages/arkit_plugin

## Firestore
Firestoreと連携するのがお手頃なので、必要ならばセッティングしときます。

## Circle CI
Gitでの事故を防ぐためにCircle CIをセッティングしてます。(使ってみたかっただけ)

実行環境にはクラウド上のコンテナまたは仮想マシンを使用し、他の一般的な CI/CD ツールと同様にDartのソースコードからアプリケーションのビルド、テストコードや
コードチェッカを利用したアプリケーションの動作テスト、アプリケーションの本番環境などへのデプロイを行えます。

ビルドできても、プルリク投げるときに警告でるかもです。
その場合は、上記のテストで違反が見つかったってことなので焦らずに解決してからもう一度プルリクを投げてね。



