---
title: "Terraform Associate合格記"
date: 2020/06/29 10:03:42
postid: ""
tag:
  - Terraform
  - 合格記
category:
  - Infrastructure
thumbnail: /images/20200629/thumbnail.png
author: 伊藤太斉
featured: false
lede: "5/24に受験したHashiCorpから出た資格の1つである、Terraform Associateを受験したときの記事になります。結果としては無事に合格したので、受験前、そして受験当日のことを今回取り扱おうと思います。"
---

# はじめに
こんにちは。TIG/DXユニットの[伊藤](https://twitter.com/kaedemalu)です。今回は、5/24に受験したHashiCorpから出た資格の1つである、Terraform Associateを受験したときの記事になります。結果としては無事に合格したので、受験前、そして受験当日のことを今回取り扱おうと思います。私はTerraform以外にも準備が必要だったので、この記事がこれから受験する人の一助となれば幸いです。
<img src="/images/20200629/1.png" class="img-small-size" loading="lazy">

# 本人のスペック
まず、はじめに受験者の私についてです。（読み飛ばしていただいて良いです）

- Terraform歴: 9ヶ月
- 他の資格:
    - AWS Solution Architect Associate
    - Google Cloud Certified: Professional Cloud Architect
- **英語**
    - そこそこ読めるけど、話す経験はほとんどない（海外経験なし）

私はフューチャーに入社して以来GCP+Terraformというコンビでインフラの作成および管理を行っていました。途中で、Google CloudのProfessional Cloud Architectを取得して、今回が2個目の資格チャレンジになります。後述しますが試験の言語が英語なので、私にとってはある意味１番のネックでした。そのため、英語の大事さを痛感した試験にもなっています。

# HashiCorp Certified: Terraform Associate とは
そもそもこの試験の内容についてざっくり中身を出しておきます。

|     | 内容 |
| ------ | ------|
| 言語 | 英語 |
| 受験方法 | オンライン |
| 試験費用 | $70.50 USD |
| 試験時間 | １時間 |
| 有効期間 | 2年間 |

受験方法は自宅からオンラインで受けられます。AWSやGCPの試験を受けたことがある方は、受験会場で画面に向かって受ける試験を自宅で行うものと考えてもらえれば良いです。試験内容は、IaCの一般的な知識から始まり、Terraformで使えるFunctionとかコマンドの挙動など概要から実践的な部分まで広く出題されます。HashiCorpから事前に[サンプル問題](https://learn.hashicorp.com/terraform/certification/terraform-associate-sample-questions)が提供されているので、出題形式を押さえるという意味で見ておくことをお勧めします。

# 試験対策
私が試験を受けるまでに行った対策と言えるものは以下になります。

- [Exam Review - Terraform Associate Certification](https://learn.hashicorp.com/terraform/certification/terraform-associate-review)
- [HashiCorp Certified: Terraform Associate Practice Exam](https://www.udemy.com/course/terraform-associate-practice-exam/)

試験ガイドはこれからTerraformの全容を知りたい人向けの[Study Guide](https://learn.hashicorp.com/terraform/certification/terraform-associate-study-guide)と、そこそこTerraformに親しみのある人向けのExam Reviewと2種類あります。私はそれなりに使ってきたぞと、自負していたので、Exam Reviewから入りました。ドキュメントの内容は試験項目別になっているので、自分が弱いと思ったところを重点的に読んだり、Function周りがまだ使い慣れていないものもあったので、`terraform console`などで一通り実行して色々試してみました。
また、Udemyの試験問題は、知識の抜け漏れがないか確かめるために買いましたが、これは結構役に立つ内容でした。1回解いて、答えを見て腹落ちするまでドキュメントなども見ながら理解を深めることをひたすら行いました。ついでに英語で読む癖をつけられたのもよかったことかなと思います。
また、TerraformとVaultとの関わりも深くまでは調べなくても、組み合わせ方は知っておいた方が良さそうでした。

# 事前準備
試験を受けるまでの流れをここでは説明していきます。少し面倒でした。

## 申し込み
[試験概要](https://www.hashicorp.com/certification/terraform-associate/)のページから申し込みます。試験自体はQuestionmarkというところが代理で行うようです。順を追っていくことで、アカウントの登録や試験ができるようになっています。試験の購入については現段階では

- Terraform Associate
- Vault Associate

の2つが購入可能です。Terraform Associateの試験を購入して、決済まで完了すると、試験時間の設定ができます。ここで結構不安だったのが、受験時の時間です。試験の選択時間はプロフィールで設定できる居住地やタイムゾーンに依存するので、試験時間を選択する前にプロフィールを確認してJSTにしておきましょう。試験官がアメリカのため、日本だと大体21時以降や、6~10時などが受験可能時間として出てきます。私は午前10時からの枠を選択しました。

## 環境
パソコン自体は順当にMacやWindowsなら受験が可能で、Webカメラやマイクがきちんと使えることを事前に確認しておくとよいでしょう。ノートPCの人はデュアルディスプレイには出来ないので、ノートPC1台と本人確認に必要なパスポートを残して机のものをすべておろしておくくらいが精神衛生上でも良いかなと思います。部屋の中はそこまで見せる必要はありませんが、他の人が絶対に入らない環境が求められますので、家族などには事前に受けることを周知しておきましょう。

# 当日
当日は試験時間の15分くらい前から試験を申し込んだページで試験の準備を進められます。ここからはリスニングとスピーキングを求められるので、私は受ける前になかなか頭を使ってしまいました。順当に試験の事前準備出来ているか（パスポートでの本人確認や机のものの整理具合)かどうかを聞かれるので、言われるがまま(あまり聞き取れてはいないのですが)進めると、試験を開始できます。
試験時間は1時間ですが、私はほとんど見直す時間がありませんでした。とりあえず、分かる問題はどんどん答えていって、あとで分からない問題に時間を使う方針で進みました。英語読むことに対して、今までで一番集中力を使った気がします。
試験を終えるとすぐに結果発表があり、そのあとはアンケートに答えます。これも終えると、試験官より声かけられて一連の流れが終わりになります。

# 結果
無事合格しました。スコアを見ると他の合格体験記と見比べて割とギリギリだったようです。今までAWSやらGCPやら受けてきましたが、また違った緊張感でした。試験終了直後は受かったというメールのみ来て、10日くらいあけるとデジタルバッジが来ます。やはり、何かしら形になるのは嬉しいですね。
合格してから数日でデジタルバッジが取得できるので、より実感が湧きます。素直に嬉しかったです。
<img src="/images/20200629/photo_20200629_01.png" class="img-middle-size" style="border:solid 1px #000000" loading="lazy">

# まとめ
試験が出されてから1ヶ月で受けましたが、とりあえず合格してよかったなという気持ちが大きく、ホッとしています。また、初の英語での受験でしたが、なんとか終えられて、個人的には結構自信がつきました。Terraformは私が触っていてとても好きなものの一つなので、勉強しながら好きなものの知識を深められることが嬉しかったです。とはいえ知識も経験もまだまだなので、これからも新しいことに挑戦しつつ、出来ることの裾野を広げられたらなと思います。
あと、英語は本当に大事であると感じたので、英語もやろうと思いました。
先日、[Terraformの入門記事](/articles/20200624/)も書きましたので、これからTerraform Associateを受験しようという方は参考にしてみてください。

## 参考リンク

- [技術ブログ Terraform一覧](/tags/Terraform/)
