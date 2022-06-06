## 米国株式市場 将来株価予測 ProbSpace コンペティション

### 主な特徴量
- ラグ特徴量（1〜4週分）
- 加重移動平均とその標準偏差
- ラグは1〜4週分
- 移動平均の間隔は52のみとした。　※もしかしたらここが大きかったかもしれない
- 単純移動平均ではなく加重移動平均を使った点、加重割合を調整した点がスコアにつながったように思われる
- 当初多くの特徴量を加えたほうがスコアが高くなると考えたが、結果は逆。
###
- 期間：2021.9.21 〜 2021.12.12
- 課題：2011/11/13～2019/11/17週の計419週間の米国株データから、2019/11/24週の終値を予測する。銘柄数は3,278。
- 評価方法：評価関数RMSLE(Root Mean Squared Logarithmic Error)
 <img src="https://latex.codecogs.com/gif.latex?\sqrt{\frac{1}{n}\sum_{i=0}^{n}(log(Pred_i+1)-log(Act_i-1))^2}" />
- データ：train_data.csv, company_list.csv, submission_template.csv

1. google-repo
 - コンペ提出用
2. train-folder
 - 練習用