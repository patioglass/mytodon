## Mytodon
## Description
コマンドラインからMastodonにいろいろするシェルスクリプト。

まだ適当に作っただけなのでトゥートできる部分しかできてない（2017/4/27）

あとシェルスクリプト初めてで試しで作ったので、おかしいところ多いかもです

一度setupを実行している人はgit pull後

    ./update

を実行してください。（mytodonコマンドの更新）
## Requirement
bash
yum install jq
## Install

    git clone https://github.com/patioglass/mytodon.git 
    cd mytodon
    ./setup		#ACCESS_TOKENを取得し、~/.bashrcに書き込み
    サーバのホスト名を登録(例：https://www.hogehoge.com):https://www.xxx.com
    ユーザ名を登録(任意の文字列):hoge
    https://www.xxx.comに登録しているメールアドレス:yyy@zzz.com
    https://www.xxx.comに登録してるアカウントのパスワード:
    % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                    Dload  Upload   Total   Spent    Left  Speed
    152   214    0   214    0    91    574    244 --:--:-- --:--:-- --:--:--  6833
    設定が完了しました。mytodon --helpを参照してください。
   
    #反映させる
    source ~/.bashrc

## Usage
   mytodon toot "トゥート！"

   mytodon -t home #タイムライン取得
