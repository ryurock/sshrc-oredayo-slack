# sshrc-oredayo-slack

SSHで接続したら俺だよってSlackで伝えるもの


## Usage

```
brew install sshrc
cat << ETX > ~/.sshrc
curl -s -X POST --data-urlencode \
  "payload={
    'channel': '#random',
    'username': 'ブーーーーンε=ε=ε=╭( ๐_๐)╮ Slackでいちいち書くのが面倒だからsshrcで伝えるよ',
    'icon_emoji': ':slack:',
    'text': 'ｿｯﾁ(*･д･)σｺｯﾁ 俺がSSH接続したポヨ'
  }" \
https://hooks.slack.com/services/xxxxxxxx >/dev/null
ETX
```


```
sshrc {ユーザー名}@IPアドレス
```
