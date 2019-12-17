# cpp-sort
 Sort algorithms implementation by C++
## はじめに
このリポジトリは、yuina_blendとnanigasi_sanによる共同開発練習用リポジトリです。  
主に以下の三点についてを目標としています。
+ C/C++でのソートをメインとしたアルゴリズムの実装
+ GitHubによる共同開発とコードレビュー、可読性を意識したコーディング
+ ~CircleCI~ GitHub Actionsを用いた自動テスト環境/CIへの慣れ

## 開発の流れ
1. ソートアルゴリズムについてのissueを立てる
1. [そのアルゴリズムの名前]と[issue番号]の入った名前のブランチを切る
  > 例：`quick-sort-12`

1. テストを書く
1. 実装していく
1. pushのたびにテストが走るので、それが通っていたら開発をすすめる、落ちたらデバッグ
1. 実装が終わったら、PullRequestを出す
1. 出されたものはコードレビューをし、問題がなければmasterにmergeする

## テストについて
今回はGitHub Actionsでテストを走らせます。  
最初はCircleCIのつもりだったんですが...はい。なんとなく使ってみたいのでこれで行きます。  
今回は以下の構成で行きましょう  
+ テストフレームワーク：Google Test(以下gtest)
+ CI環境：GitHub Actions
+ 参考資料：[GitHub Actionsを使ってみた - Qiita](https://qiita.com/toppy-luna/items/8358c19bbfb2aee4e848)

gtestの書き方については以下を参考にします  
+ [Googletest Primer](https://github.com/google/googletest/blob/master/googletest/docs/primer.md)  
+ [Googlte Testを導入してみた - Qiita](https://qiita.com/y-vectorfield/items/6238cfd2d9c34aefe364)  

テスト項目については網羅的にテストをしているかを考えながらやっていきましょう。カバレッジは面倒なので序盤はやりません。