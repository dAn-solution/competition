## [【第19回_Beginner限定コンペ】国勢調査からの収入予測](https://signate.jp/competitions/576)

- 最初LightGBMを使って実行したが合格ラインには届かなかった
- 次にRidge回帰、ランダムフォレスト、CNNを試みたが合格ラインには届かず
- GBDT（勾配ブースティング木）のtrain試験でも数値が高かったのでこれを採用
- LightGBMばかりに囚われたが、他のモデル同様に扱わなければいけない