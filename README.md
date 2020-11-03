cloudformation による、AWS ECS環境の構築スクリプト
概要
このスクリプトは、AWS ECSをマルチAZで構築するcloudformationスクリプトです。

以下の構成を構築できます。
---
構成図
![aws構成図](https://user-images.githubusercontent.com/30540542/98032856-f8cb6780-1e57-11eb-8865-7a1fef3b8038.jpg)
---
ECRの構築、及びdockerイメージのデプロイは、本スクリプトでは記述しておりませんので、事前に準備が必要です。
ECSはプライベートサブネットに構築し、Natゲートウェイでインターネットへ通信可能としています。
コンテナイメージのCI/CDはCircleCIを使用しております。「nginx-sample」リポジトリを参照ください。
