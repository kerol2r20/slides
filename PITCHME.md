## NLP WITH Deep Learning
### Yu-hsin Lu
### 2017/12/03

---

## Tools
1. Jieba 分詞
1. Word2Vec 量化
1. RNN(LSTM)
1. GAN
1. Seq2Seq

---

## Case study

---

### Word2Vec
將詞彙(word)投影到一個高維度的平面上，如果兩詞彙之間的距離越近，代表兩詞彙的意義越相近。

+++

#### 訓練方式
訓練大量文章之**前後文**，找到詞彙之間對應的平面關係。

+++

![](http://mccormickml.com/assets/word2vec/training_data.png)

+++

#### 訓練成果
1. 找到相似詞

![](https://raw.githubusercontent.com/dominiek/word2vec-explorer/master/public/screenshots/tsne-10k.png?size=auto)

+++

1. 找到詞彙之間的相對應關係
 1. 研究生：實驗室 = 公務員：？ Ans: 辦公室
 1. 老師：學生 = 主管：？ Ans： 員工

+++

