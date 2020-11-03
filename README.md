cloudformation による、AWS ECS環境の構築スクリプト
概要
このスクリプトは、AWS ECSをマルチAZで構築するcloudformationスクリプトです。

以下の構成を構築できます。

構成図
![aws構成図](https://user-images.githubusercontent.com/30540542/98032113-db49ce00-1e56-11eb-8032-6033567cef28.JPG)
---
ECRの構築、及びdockerイメージのデプロイは、本スクリプトでは記述しておりませんので、事前に準備が必要です。
ECSはプライベートサブネットに構築し、Natゲートウェイでインターネットへ通信可能としています。
コンテナイメージのCI/CDはCircleCIを使用しております。「nginx-sample」リポジトリを参照ください。
