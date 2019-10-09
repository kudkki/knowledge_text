# オペレーション

## 一読
* [仕事を任せられるエンジニアになるために意識してほしいこと](https://tech.tabechoku.com/entry/2019/05/02/182457)
* [リリース手順書について本気出して考えてみた](http://road-to-king.hatenablog.com/entry/2014/02/17/%E3%83%AA%E3%83%AA%E3%83%BC%E3%82%B9%E6%89%8B%E9%A0%86%E6%9B%B8%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6%E6%9C%AC%E6%B0%97%E5%87%BA%E3%81%97%E3%81%A6%E8%80%83%E3%81%88%E3%81%A6%E3%81%BF%E3%81%9F_%23Clea)

## 前提知識
* [Linux標準教科書](https://linuc.org/textbooks/linux/)
* [The Art of Command Line](https://yakst.com/ja/posts/2545)

## リリース作業の前提知識
* 手順書の罠
    * 手順の意味 求める結果 成否の確認 などが省略される
* コピペ作業の罠
    * 行末の改行 全角の空白文字や制御文字
    * 文字コード
* 並行作業の罠
    * 自分が今どこにいて何をしてたサーバに何をするのか
* サービス特性の罠
    * サービスを継続させているかどうか把握できてるか
    * サービスを止めたマシンだけを処理することができてるか

## ssh/shell/screen一般教養
* ssh
    * 公開鍵認証 ssh-agent
    * ターミナルソフト 鍵転送 スクロールバッファ
* bash
    * emacsキーバインドで素早く正確に操作
    * bashrc ailias
* screen  
  [SCREEN](https://linuxjm.osdn.jp/html/GNU_screen/man1/screen.1.html)  
  [GNU Screen](https://wiki.archlinux.jp/index.php/GNU_Screen)
    * 複数window マルチsshして並行コマンド実行


## 負荷分散について
* ロードバランサとは
  [「Linux Virtual Server」と「Keepalived」で作る冗長化ロードバランサ](https://knowledge.sakura.ad.jp/274/)
* vipの作り方
  [IDCFクラウドでkeepalivedを使ったLVS構築(1)](https://blog.idcf.jp/entry/cloud/keepalived/)
  [IDCFクラウドでkeepalivedを使ったLVS構築(2)](https://blog.idcf.jp/entry/cloud/keepalived2/)
* サービスインサービスアウト  
ヘルスチェック


## パッケージマネージャについて
* rpm yum  
[rpm と yum を今更理解したい](https://qiita.com/spadeloves/items/2d829e33d7a9c1b36923)

## CI/CDについて
* chefが実行される仕組み

## 監視について
* nagiosの基本

## メモ
* screenでなくtmuxが使える場合  
tmuxマルチssh 複数サーバへ同時接続して作業  
  [tmux + ssh + Mackerel API を組み合わせたとにかくモダンなサーバオペレーション](https://blog.yuuk.io/entry/tmux-ssh-mackerel)
* [Linuxサーバでカジュアルに作業ログを取得する方法](https://qiita.com/keigodasu/items/3eebbc079274ad8dd2c2)