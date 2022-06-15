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

プルリクするためにsshを作成して登録  
`ssh-keygen`  
作成したssh**公開鍵**をgithubに登録（settings -> ssh and gpg keys）  
また、.sshフォルダの中にconfigを作成して以下を記載（記載しないとpermissionになるかも）  
Host github.com  
HostName github.com  
IdentityFile ~/.ssh/作成したssh鍵名  
User git  
  

