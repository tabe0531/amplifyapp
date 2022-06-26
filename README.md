# 参考サイト

https://aws.amazon.com/jp/getting-started/hands-on/build-react-app-amplify-graphql/module-one/?e=gs2020&p=build-a-react-app-intro

# 学習内容

新しい React アプリケーションを作成する  
GitHub リポジトリを初期化する  
アプリを AWS Amplify でデプロイする  
コードの変更を実装してアプリを再デプロイする

github に登録  
新しいレポジトリの作成

`git init`  
`git remote add origin git@github.com:登録名/レポジトリ名.git`  
`git add .`  
`git commit -m “initial commit”`  
`git push origin master`

プルリクするために ssh を作成して登録  
`ssh-keygen`  
作成した ssh**公開鍵**を github に登録（settings -> ssh and gpg keys）  
また、.ssh フォルダの中に config を作成して以下を記載（記載しないと permission になるかも）  
Host github.com  
HostName github.com  
IdentityFile ~/.ssh/作成した ssh 鍵名  
User git

# プッシュ後の自動デプロイ

初回デプロイに時間がかかるのと、プッシュ後の自動デプロイでも結構時間がかかる（ビルドが）  
master ブランチを指定してデプロイしているので、develop とかでプッシュすると話は別そう

# Amplify CLI をインストール

アプリの AWS クラウドサービスを作成するため統合ツール  
Amazon IAM を使用すると、AWS でユーザーとユーザーアクセス許可を管理できる
