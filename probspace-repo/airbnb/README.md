## airbnb／[民泊サービスの宿泊料金予測](https://comp.probspace.com/competitions/bnb_price/ranking) ProbSpace コンペティション
- 期間：2022.2.28 〜 2022.5.8
- 課題：最寄り駅の位置情報などをもとに国内の民泊施設の料金を算出する。
- 評価方法：RMSLE
 <img src="https://latex.codecogs.com/gif.latex?\sqrt{\frac{1}{n}{\sum_{i=1}^{n}{(\log(Pred_i+1)-\log(Act_i+1))^2}}}" />
- データ：- 訓練データ(train_data.csv)
		 - テストデータ(test_data.csv)
		 - 東京都23区内駅緯度経度データ(station_list.csv)
         - サンプルサブミット用データ(submission.csv)


1. google-repo
 - コンペ提出用
2. train-folder
 - 練習用