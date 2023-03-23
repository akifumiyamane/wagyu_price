# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？
- リモートリポジトリ
- ネット上に配置して複数人で共有するためのリポジトリ
- GitHub以外にGitLabやBitBucketがある

- ローカルリポジトリ
- 開発者一人ひとりが使用するために自分のPC上に配置するためのリポジトリ


## プッシュとマージの違いは何でしょうか？
- pushはローカルリポジトリの変更をリモートリポジトリに反映させる
- マージは切ったブランチを一つのブランチと統合する、

## コミットとプッシュの違い
- コミットはローカルリポジトリに変更を反映させる
- プッシュはリモートリポジトリに反映させる
- コミットでローカルに変更を反映させプッシュでローカルの変更内容をリモートに送信する


## コミットのメッセージはどのように書いてあげるのが最適でしょうか？
- 一目で変更内容がわかるように書く
- 「何を」と「なぜ」を書く
- prefix (接頭辞)をつける


## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？
- コードレビューを挟んでからマージする

- ローカルでマージするフロー
- コードにバグがある時に気づかない可能性があるのがデメリットでローカルもリモートも変更内容が反映されて手順が少なくなるのがメリット

- プルリクエストでマージするフロー
- コードレビューしてからマージするので事前にバグが発見しやすいのがメリットでリモート上でマージした内容を、ローカルのmasterブランチは知らないのでローカルに変更を反映させる必要があり手順が増えるのがデメリット


## コンフリクトを起こしてしまった場合、どう対処すべきですか？
- 先にマージされた変更内容を取り込む
- 後にマージしようとしている変更内容を取り込む
- どちらの変更内容も取り込む
- 三つのうちどれを選択するかは取り込みたい内容で判断する
- 複数人で同じファイルを編集しない
- commit したり stashしたりして変更中のファイルの状態をなくしておく
- pullするときは、pullするブランチに移動してからpullする

