# install-wordpress-to-aws
AWSへWordPressをインストールする、ベストプラクティスに沿ったシステムを構築します

## 使い方

1. source/formation.ymlを用いて、ソースのためのAmazon S3バケットを作成します
2. plugins以下を1で作成したバケットのplugins以下にアップロードします
3. image/formation.ymlを用いて、イメージパイプラインを作成します
4. 3で作成したイメージパイプラインを用いて、AMIを作成します
5. main/formation.ymlを用いて、WordPress環境を構築します
