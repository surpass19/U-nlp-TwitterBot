# U-TwitterBot
人工知能（AI）を搭載したTwitterボットを作ろう【Seq2Seq+Attention+Colab】<br>
https://www.udemy.com/course/twitter-bot/

# 学んだこと
* TwitterAPI
  * ツイートの取得(人, ワード, トレンド)
  * POST
* word2vec
  * CBOWまたは, Skip-gramというNNが用いられる
* Seq2Seq
  * 時系列変換のモデル
    * 機械翻訳
    * 文章要約(本文 ⇨ 要約)
    * 対話(自分 ⇨ 相手)
* + Attention
* Bidirectional RNN
* 自然言語(応答文)のデータ拡張 <br>
他の水増しの前処理（Augmentation、オーグメンテーションと言います）としては、下記リンク先が参考になるかと思いますので是非ご一読ください。<br>
https://qiita.com/tchih11/items/aef9505d26d1bf06a04c
* 応答文の作成
* 単語同士の演算
  * U-Word-vec.ipynb

# キーワード
* TwitterAPI
* API Keyをjsonで隠す
* API Keyをpythonで隠す
* Pytorch
* RNN
* Seq2Seq
* エンコーダーデコーダー
* 自然言語処理
  * word2vecを用いた学習
  * Janomeを使って分かち書き
  * 単語同士の演算
    * コサイン類似度

# 今後やりたいこと
Attentionの利用により精度が高まりましたが、LSTM/RNNで時系列データを逐次的に処理しているためデータの並列処理ができず高速化ができない課題は解決されていないままでした. 2017年にGoogle社が発表した「Attention is All You Need」という論文で、RNN/LSTMおよびCNNを用いず、「Attention」のみを用いた「Transformer」を提案し、従来のモデルで抱えていた「高速化ができない」、「精度の高い依存関係モデルを構築できない」という課題を解決しました。
Transformerは、昨今のBERTやGPT2/GPT３といった最新のＮＬＰモデルの基礎モデルであり、またDETR（別冊で掲載予定）などの画像認識にも使われている重要なモデルです。
https://qiita.com/DeepTama/items/20b93ff8b8547428f662
