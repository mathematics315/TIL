# Git Command

## stash
変更済みファイルを一時退避させる。  
主に変更した点を元に戻さずに他ブランチへチェックアウトしたいときに用いる。  

```
$ git stash save
```

上記コマンドで現在の変更点を一時退避することができる。  

```
$ git stash list
```

上記コマンドでstashしたstashを見ることができる。

__-p__ オプションを用いることで

変更した __内容__ を見ることが可能

```
$ git stash apply stash@{0}
```

__apply__ 以降は一時退避した変更を戻したいstash名を入力する。


```
$ git stash drop stash@{0}
```

stashは __apply__ しただけでは削除されずにそのまま残る。
不要になったstashは削除する。

```
$ git stash pop stash@{0}
```

stashを適用して削除する。
これが一番便利かもしれない。
