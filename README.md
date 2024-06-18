# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
* リモートリポジトリとはネット上に配置して複数人で共有するためのリポジトリのことでGitHubなどのリモートリポジトリを提供するサービスがある
* ローカルリポジトリとはPC上に配置するためのリポジトリのことで開発者が使用するためのもの。


## プッシュとマージの違いは何でしょうか？
* マージは切ったブランチの変更履歴を他のブランチに取り込むために使用するコマンドのことで２つのブランチを統合すること。
プッシュとはリモートリポジトリとローカルリポジトリは自動で同期されるわけではなく、ローカルのmasterブランチをリモートリポジトリに反映させるためのコマンド。



## コミットとプッシュの違い
* コミットとはゲームなどでいうセーブのようなもの。
git addコマンドでステージングしたものの変更履歴を保存するためコマンドで
プッシュはゲームで言うところのセーブデータ別のものにコピーするようなもの。
コミットした箇所までのローカルリポジトリの内容をリモートリポジトリに反映させるためのコマンドで目的が違うコマンドである。
プレフィックスの例としてfix(バグ修正)やadd(ファイルや機能の追加)delete(ファイルの削除)など
例）fix: 〇〇のエラーが起きているため××に修正しました。　

## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
* 第三者が見てもどこをどのように変更したのかが分かるように書くことが重要で
また、プレフィックス（接頭辞）をつけることでコミットメッセージに含める情報を明確にすることができる。

## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
* 開発者１人ではなく、アップされるまでに第３者が介入するかしないかの違いがある。
ローカルでマージする方法だと作業内容をコミットしmasterにマージをし、そのままリモートへプッシュするという流れになるが、プルリクエストでマージする方法はレビュー担当者の目が入るためコードにバグ等があった場合、アップされる前に発見できる確率がグッと上がるためバグがそのままアップされてしまう可能性が低くなる。


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
* コンフリクトが発生した場合は以下の３つの方法で変更内容を取り込む。
1. 先にマージされた変更内容を取り込む
2. 後にマージしようとしている変更内容を取り込む
3. どちらの変更も取り込む

また、チーム開発の中でコンフリクトは起きてしまうことがある。
チーム開発でコンフリクトが起きてしまった場合は、１人で勝手に対処はせずに
チームとのコミュニケーションを密にとり、冷静にどう対処をすべきかを話し合うことが大切です。
