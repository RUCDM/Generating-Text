# Generating-Text
## 本模型使用的数据
* Amazon_beauty
* Amazon_Clothing_Shoes_and_Jewelry
* Amazon_Office_Products
* JD Data

### 生成文本：
| Input                         |output                                                                                  |
|:-----------------------------:|:--------------------------------------------------------------------------------------:|
|this is a well built calculator|this is a well built calculator to and and but the glue inkjet cardboard have the greasy|
|i have a canon powershot       |i have a canon powershot so are not other color magnets. white or want to my that the of ivory is buy very magnets.|
|i wanted to make sure that     |i wanted to make sure that machine it's experience am file ink or you're made directly nature very that once at is medium sense.|

### 生成的模板：
| pattern                   |
|:-------------------------:|
|and NN i VBP the NNS       |
|a NN i VBP JJ the          |
|and have NN i JJ NNS       |
|this is NNS NN             |
|a good NN JJ               |
|i had NN JJ                |
|...                        |

### 生成的莎士比亚诗词：
| Input                         |output                                                                                  |
|:-----------------------------:|:--------------------------------------------------------------------------------------:|
|时间已经终止它的运行了           |时间已经终止它的运行了处置必须，神座没有吧不的能手你你们吧罗她神座分庭抗礼守戒呼吸啊智慧向我此上还有女儿什么虽然举动这小书罗我要是话有不宽容点儿米兰达。|

### 生成的京东评论（今天上午刚跑出来）：
| Input                         |output                                                                                  |
|:-----------------------------:|:--------------------------------------------------------------------------------------:|
|价格便宜，物流也给力             |不好送朋友家但是但是满意                                                                  |
|京东不错！唇膜很棒！             |干净没有放心扣头好吧不错经常很味道                                                         |
|物美价廉，很不错                 |物美价廉，很不错关键吧很满意                                                              |

### 实验分析：
#### 实验结论：
相较上周的模型，本模型主要在层数以及迭代次数上有所增加，上图是迭代420次的的结果。虽然从结果看效果还是不理想，但整体的句子骨架已经出来了，句子中的部分词语之间也存在了相关性。例如，输入this is a well built calculator，虽然后面句子没有产生关于计算器的描述，但是生成了glue inkjet cardboard have the greasy，表示蓝色墨水盒很润滑。
#### 实验问题：
相比较古诗生成、莎士比亚诗句生成，从实验数据上来看，Amazon的数据噪声比较大，从肉眼来看，很多训练的评论数据根本不能成为一句通顺的话，导致预测结果不是很理想。此外，从重现古诗生成以及莎士比亚诗词生成的结果来看，其实他们的实验结果有一些“水分”，并不能生成通顺的句子，只是能生成相似风格的语言。*因此，下一周我打算换一批数据集进行尝试，

并将生成的模板和2-gram应用到模型中。
