# Phaserのサンプルを動かす手順
- VirtualBoxを起動して、Lubuntuを起動
- 左下の[スタート]メニューをクリックして、[実行]をクリック
- `lxte`(エル・エックス・ティー・イー)と入力すると、[LXTerminal]が表示されるので、[Enter]キーを押して起動
- 端末が起動したら、以下を入力していく
```
cd phaser
cd phaser-examples
cd examples
http-server
```

以上で、ホームフォルダー内の`phaser/phaser-examples/examples`フォルダーに移動して、HTTPサーバーが起動される。

Webブラウザーで `http://localhost:8080/sideview.html` を開くと、サンプルビュアーが表示される。左のメニューから[Game]>[Starstruck]をクリックすると、サンプルのゲームが実行できる。

# 修正したら・・・
画像やマップなどのリソースを変更した場合、通常のリロードでは変更が反映しない。以下の手順で、キャッシュとハード再読み込みを行う。

- [Fn]+[F12]キーを押して、開発者ウィンドウを表示（すでに表示されていたらこの手順は不要）
- リロードアイコンを長押しする
- メニューが表示されるので、一番下の[キャッシュの消去と再読み込み」を選択

以上で、古いリソースが削除されて、再読み込みされる。左のGame欄から[StarStruck]をクリックして実行すると、画像がさし変わる。

