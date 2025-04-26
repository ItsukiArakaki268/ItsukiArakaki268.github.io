+++
title = 'ssh-agentの使い方'
date = 2023-10-26T12:32:45+09:00
draft = false
tags = ["ssh"]
+++

GitHub に push する際、ssh-agent の使い方で躓いたのでメモがわりに。

<!--more-->

## ssh-agent の起動

```
$ eval `ssh-agent`
```

## ssh-agent の停止

```
$ ssh-agent -k
```

## ssh-add の使い方

秘密鍵を ssh-agent に登録。

```
$ ssh-add [秘密鍵のパス]
```

登録されている鍵の公開鍵一覧を表示。

```
$ ssh-add -L
```

登録されている鍵を削除。

```
$ ssh-add -d [秘密鍵のパス]
```
