## NLP WITH Deep Learning
### Yu-hsin Lu
### 2017/12/03

---

## Tools
1. Jieba
1. Word2Vec
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

+++

##### 找到相似詞

![](https://raw.githubusercontent.com/dominiek/word2vec-explorer/master/public/screenshots/tsne-10k.png?size=auto)

+++

##### 找到詞彙之間的相對應關係
 1. 研究生：實驗室 = 公務員：？ Ans: 辦公室
 1. 老師：學生 = 主管：？ Ans： 員工

+++

#### Word2Vec不足點
Word2Vec不知道整句句法的前後文關係，它是面向單詞的訓練方式，不是面向語句。

---

### Sentiment Analysis
給與機器一段文字，讓機器判斷某種Feature的強度，例如： 某句話正面負面，開心難過......

+++

#### 訓練方式
Feature: 語句  
Label: 某種情緒的分數  
利用LSTM的方式進行訓練

+++

#### 訓練成果
1. It is bad => *0.05*
2. It is not bad => *0.9* |
3. AI is hard to learn, but it is powerful => *0.86* |
4. AI is powerful, but it is hard to learn => *0.35* |
5. AI is powerful even though it is hard to learn => *0.73* |

---

#### Summarization
給予文章，自動訓練出文章摘要。

+++

##### 訓練方式
Feature: 新聞內文  
Label: 新聞標題  
使用Seq2Seq+LSTM的方式訓練出Model

+++

##### Seq2Seq
![](https://i.imgur.com/Vlm0rBw.png)

---

## 瓶頸
1. 問題定義
2. 資料量
3. 訓練設備
