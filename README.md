## Git Ordered Merge

### 概要
Gitにおいて、ファイルやディレクトリをmergeする順序決めを可能にします。
現仕様ではリモートリポジトリからのmergeのみをカバーしています。

### Useage

#### コマンド
git-ordered-mergeというファイルをPATHの通っている場所に置く、
またはPATHを通す事によってコマンドを使用することができるようになります。
```
$ git ordered-merge <remote> <branch> 
```

#### 順番の決め方

mergeしようとしているプロダクトルートに入っている、.git内に設定ファイルを追加することで順序を決めることができます。
`.git/info/checkout-order`というファイルを追加してください。

例
.git/info/checkout-order
```
server/
assets/
client/
.
```

上記の例は、上から順番にmergeされて最終的に`.`によってカレントディレクトリ内のすべてのファイルをmergeする記述です。
