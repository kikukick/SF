```markdown
<ins>**概要**</ins>
参加者は配布プリントに沿って下記の手順で「擬似クッキーハッキング→成りすましログイン」を体験し、セキュリティの基本を学びます。
## CMD:0（初心者モード）
start   → start cookie
visit   → open page
get     → get cookie
install → install brute
crack   → crack pin
login   → login id=<correct_pin>
unlock  → output cookie
## CMD:1（上級者モード）
start   → src cookies-output-attack go
visit   → src file://public_resource?id=875
get     → src get cookies-for-id=875
install → pip install hackkit
crack   → src ~/attack/model/bruteforce/0000-9999
login   → src use sessionid=<correct_pin>
unlock  → cookie print from date library
#===操作手順===
保護者役がアカウントを作成
参加者に交代し、ターミナルでモードを指定して起動：
python start.py --set 0   ##　初心者モード
python start.py --set 1   ## 上級者モード
help または help! で次のコマンドを確認しながら順次実行。
install→crack→login で擬似ブルートフォース体験。
unlock で得たクッキー情報をフォームに入力し、ログイン成功！===動作確認と互換について===
## 必要環境
macOS 15.5以上、Python 3.x
pip install flask

## サーバー起動例
python start.py --set 0 ## 初心者モード
Flaskベースのローカルサーバー（127.0.0.1）で動作
Python 3.x 以降対応
#===安全性と合法性===
すべてローカル環境（外部通信なし）で完結
実データ・実ユーザー情報は使用せず、擬似データのみ
学習目的の体験演出であり、外部攻撃は一切行いません
バックドアなんて仕込んでないよ
XSSもないよ
信じろ！知らんけど
