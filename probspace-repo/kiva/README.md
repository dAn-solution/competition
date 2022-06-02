## [Kiva／クラウドファンディングの資金調達額予測](https://comp.probspace.com/competitions/kiva2021) ProbSpace コンペティション
- 期間：2021.11.15 〜 2022.2.13
- 課題：2018,19年の過去2年の融資実績を訓練データとして、2020,21年の融資額を予測
- 評価方法：MAE(平均絶対誤差)
 <img src="https://latex.codecogs.com/gif.latex?\frac{1}{n}\sum_{i=0}^{n}|\hat{y_i}-y_i|" />
- データ：
         - 訓練テーブルデータ(train.csv)
		 - 訓練画像データ(train_images.zip)
		 - テストテーブルデータ(test.csv)
		 - テスト画像データ(test_images.zip)
         - サンプルサブミット用データ(sample_submission.csv)


1. google-repo
 - コンペ提出用
2. train-folder
 - 練習用