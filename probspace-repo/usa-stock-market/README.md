## 米国株式市場 将来株価予測 ProbSpace コンペティション
- 期間：2021.9.21 〜 2021.12.12
- 課題：2011/11/13～2019/11/17週の計419週間の米国株データから、2019/11/24週の終値を予測する。銘柄数は3,278。
- 評価方法：評価関数RMSLE(Root Mean Squared Logarithmic Error)
   $$
   \sqrt{\frac{1}{n} \sum_{i=0}^{n}(log(Pred_i + 1) - log(Act_i - 1))^2}
   $$
- データ：train_data.csv, company_list.csv, submission_template.csv