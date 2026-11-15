# heisei_hompe_02
BBSをサーバにつないだよ

## ホームページ

VS CodeのLive Serverなどで `heisei_hompe_02.html` を配信すると確認できます。Firebase未設定時は、BBSの投稿を開いているブラウザー内に保存します。

## Firebase掲示板の設定

1. Firebase Consoleでプロジェクトを作成し、ウェブアプリを登録します。
2. Cloud Firestoreを有効にします。
3. `heisei_hompe_02.html` 内の `firebaseConfig` を、Firebase Consoleに表示されるウェブアプリの設定値に置き換えます。
4. Firestoreのセキュリティルールで、`bbs-posts` コレクションへの読み書きを適切に制限・検証してください。公開掲示板として使う前に、スパム対策も設定してください。

設定後は、VS CodeのLive Serverなどでページを配信して確認してください。Firebaseを使う場合、Firestoreの設定やルールに問題があると投稿・読み込み時に画面へエラーが表示されます。
