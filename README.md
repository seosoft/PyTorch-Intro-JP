# 手順

以下の通り実行します:

1. [日本語版ワークショップ](https://github.com/seosoft/PyTorch-Intro-JP) の GitHub リポジトリ にアクセスします。
2. [Clone or download] で Clone 用の URL を取得します。（クリップボードにコピーします）
3. [Azure Notebooks](https://notebooks.azure.com) に接続してサインインします。
4. ML と PyTorch について学ぶために start.ipynb を実行します。
5. Azure ML サービスについて学ぶために cloud.ipynb を実行します。


# Machine Learning クイックスタート

この簡単なチュートリアルの目的は、機械学習プロセスにあなたを集中させることです。 機械学習（ML）は、実行については「コード」とほぼ同じ方法で実行されますが、作成については基本的に「コード」とは別の方法で作成します。主な違いは、機械学習では「学習する」必要がある固定パラメータを持つ実行パスのクラス（通常モデルと呼ばれる）が設定されていることです。 教師あり学習では、これらのパラメータは ML アルゴリズムに入力と答えの例を与えることによって最適化されます。プロセスは通常、次のように進めます。

1. 質問から始める
2. 適切なデータを探す
3. データから適切な項目を選択する
4. モデルの種類を選択する
5. モデルのパラメーターを最適化する
6. モデルを保存する
7. モデルを製品として配置する

このリポジトリで紹介されているノートブックは2つのセクションに分かれています:

- 問題、データ、実験 - ローカル
- 大規模な実験、デプロイ - クラウド

# ローカル
最初のノートブック (start.ipynb) は、機械学習プロセスへのローカルでのアプローチを示しています。このノートブックでは、上の最初の5つのステップがありますが、小規模です。（この場合、問題はそのまま小さくなります。一般に、大規模な問題に取り組みには、小さなスケールで始めて、仮設の一部が証明されたら、大規模にしていきます）

# クラウド
could.ipynb は、Azure Machine Learning Service を使用する大規模なアプローチについて説明し、上記の手順 4～7 について説明します。この場合、データセットのサイズは全く変更されておらず、問題なくローカルで実行できますが、利用可能なすべてのデータのごく一部についてローカルでテストしてから仮説をフルデータセットでテストするシナリオを考えます。

# 問題
機械学習を学ぶプロセスを考えた結果、機械学習の「Hello, World」で進めます。 **数字の予測** です。

![数字の例](images/digits.png)

基本的に、28x28ピクセルのグレースケール画像で、実際の手書きの数字を予測できるでしょうか？数学的に言いかえれば、0～255の数字の784サイズのベクトルを与えられれば、対応する数字を返すことができるでしょうか？

# 質問と提案
このノートブックに理解しにくい部分がある場合は、リポジトリに問題を追加してください。これを、とても理解しやすいものにしたいと思います。私の個人的な意見は、誰もが起こっていることの基本を理解できるということです！
