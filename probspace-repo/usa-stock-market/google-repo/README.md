## 米国株式市場 将来株価予測 ProbSpace コンペティション
- 期間：2021.9.21 〜 2021.12.12
- 課題：2011/11/13～2019/11/17週の計419週間の米国株データから、2019/11/24週の終値を予測する。銘柄数は3,278。
- 評価方法：評価関数RMSLE(Root Mean Squared Logarithmic Error)
 <img src="https://latex.codecogs.com/gif.latex?\sqrt{\frac{1}{n}\sum_{i=0}^{n}(log(Pred_i+1)-log(Act_i-1))^2}" />
- データ：train_data.csv, company_list.csv, submission_template.csv

1. Probstock005.jpynb
 - はじめは時系列データであるのでARモデルARIMAモデルを構築してはどうかと実施
 - しかしPublic Scoreが0.04938と悪く、次のLightGBMへ

2. Probstock007.jpynb
 -  コンペ参加者の[DT-SN](https://comp.probspace.com/users/DT-SN/0)さん公開の「[LightGBM Base line(LB=0.03781)](https://comp.probspace.com/topics/DT-SN-Posta3d47ae1bcea01c64bd5)」を（大いに）参考
 - ARIMAモデルを提出してから、別の勉強をしていてやり直しが12月1日から
 - 時間的なこともあるがLightBGMが初めてということもありその解読に力点
 - 特徴量とパラメタのチューニングに時間をかけた
#### 感想
 - 2位になったshoji9x9さんの[解法](https://github.com/shoji9x9/StockPricePrediction)を見ると、lightGBMを同じく使っているとはいえ、私が思っていた以上に深く分析をしている
 - 開発途中で「シンプルな方が良いのか？」と思っていたけれど、0.03692と0.03724の差はこういったところか
 - とはいえ参考元の DT-SNさんが0.03741だった事をみると特徴量の選択、パラメタのチューニングの試行錯誤は大胆さが必要かとも感じた