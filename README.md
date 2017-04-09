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
| pattern                   |
|:-------------------------:|
|and NN i VBP the NNS       |
|a NN i VBP JJ the          |
|and have NN i JJ NNS       |
|this is NNS NN             |
|a good NN JJ               |
|i had NN JJ                |
|...                        |

### 实验分析：
#### 实验结论：
相较上周的模型，本模型主要在层数以及迭代次数上有所增加，上图是迭代420次的的结果。虽然从结果看效果还是不理想，但整体的句子骨架已经出来了，句子中的部分词语之间也存在了相关性。例如，输入this is a well built calculator，虽然后面句子没有产生关于计算器的描述，但是生成了glue inkjet cardboard have the greasy，表示蓝色墨水盒很润滑。
