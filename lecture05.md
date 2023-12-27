# 第5回課題報告

### サンプルアプリケーションをEC2上にデプロイして動作させる、サーバーアプリケーションを分ける

- 組み込みサーバーだけで表示

![画像](image05/lect05puma.png)

- サーバーアプリケーションを分けて表示

![画像](image05/lect05NginxUnicorn.png)

### ALBを追加、動作確認

- ALB詳細

![画像](image05/lect05alb-1.png)

- ターゲットグループ詳細

![画像](image05/lect05alb-2.png)

- 登録済みターゲット

![画像](image05/lect05alb-3.png)

- 動作確認

![画像](image05/lect05alb-4.png)

### S3を追加、動作確認

- s3fs-fuseを使用し、S3バケットを直接マウントしました。画像の保存先をS3に変更しました。

![画像](image05/lect05s3-1.png)

![画像](image05/lect05s3-2.png)

- 保存した画像

![画像](image05/lect05s3-3.png)

### 構成図

![画像](image05/lect05diagram.png)

### インフラストラクチャー構成とセキュリティ概要

- VPC詳細

![画像](image05/lect05vpc.png)

- EC2詳細

![画像](image05/lect05ec2.png)

- RDS詳細、接続とセキュリティ

![画像](image05/lect05rds-1.png)

![画像](image05/lect05rds-2.png)

- セキュリティーグループ

![画像](image05/lect05sg-1.png)

![画像](image05/lect05sg-ec2.png)

![画像](image05/lect05sg-rds.png)

![画像](image05/lect05sg-alb.png)

- ※アウトバウンドは全て許可しています。

