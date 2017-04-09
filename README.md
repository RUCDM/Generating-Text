# Generating-Text
## 本模型使用的数据
* Amazon_beauty
* Amazon_Clothing_Shoes_and_Jewelry
* Amazon_Office_Products

### 生成文本：
| Input                         |output                                                                                  |
|:-----------------------------:|:--------------------------------------------------------------------------------------:|
|this is a well built calculator|this is a well built calculator to and and but the glue inkjet cardboard have the greasy|
|i have a canon powershot       |i have a canon powershot so are not other color magnets. white or want to my that the of ivory is buy very magnets.|
|i wanted to make sure that     |i wanted to make sure that machine it's experience am file ink or you're made directly nature very that once at is medium sense.|

### 生成的模板：
| Input                 | Precison      |    Recall    |  F-Measure   | settings                                  |
|:-------------------------:|:-------------:|:------------:|:------------:|:-----------------------------------------:|
|docvec+title+LDA+SVM       |0.801155292901 |0.803142857143|0.802147843826|128D doc2vec+128D title-word2vec+100D LDA  |
|docvec+SVM                 |0.729639110528 |0.733142857143|0.731386787639|128D doc2vec                               |
|word2vec+CNN               |0.671994335198 |0.653571428571|0.662654859761|128D word2vec                              |
|word2vec+SimpleRNN         |0.480495854176 |0.477857142857|0.479172865827|128D word2vec                              |
|word2vec+LSTM              |0.646029423882 |0.641428571429|0.643720776866|128D word2vec                              |
