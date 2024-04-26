# duanDataMining
# 1.注册github用户

## 1.1首先进入github官网

## 1.2点击右上角注册按钮sign up，来到注册页面
![图片1](https://github.com/duanruixia/duanDataMining/assets/167868610/54596890-c001-42dc-b4ff-128b680644c6)

## 1.3在光标处输入自己的邮箱，邮箱必须是可以收到邮件的

<img width="957" alt="图片2" src="https://github.com/duanruixia/duanDataMining/assets/167868610/6710d6cc-ac79-4713-96d9-918e5d37e058">



## 1.4点击Continue，继续在光标处创建密码，继续创建用户名

## 1.5进行相应的验证，点击creat account后，会出现这个界面

![图片3](https://github.com/duanruixia/duanDataMining/assets/167868610/4b13c319-14f3-4df4-a5c3-13485a55a6dd)


## 1.6这时邮箱就会收到一封邮件，输入邮件中的数字页面会自动跳转

## 1.7根据自身情况进行相应个性化设置

![图片4](https://github.com/duanruixia/duanDataMining/assets/167868610/a56a1e63-6ab6-4c7f-8683-bf726845bb2e)


## 1.8到这个界面时，GitHub便创建好了

<img width="946" alt="图片5" src="https://github.com/duanruixia/duanDataMining/assets/167868610/63db1875-28a2-4759-90b0-56658265e437">

# 2.建立一个库duanDataMining

## 2.1点击右上角的加号，选择new repository,取名为duanDataMining

![图片6](https://github.com/duanruixia/duanDataMining/assets/167868610/b8cba5fa-1f1b-4943-a4ee-656566fb52e9)

<img width="728" alt="图片7" src="https://github.com/duanruixia/duanDataMining/assets/167868610/ed804e25-5d90-426e-99b8-a16ec12c8351">



# 3.上传自己的PPT到duanDataMining

## 3.1进入自己的库，选择右上角的加号，选择upload files，然后将ppt拖进去，之后点击提交
<img width="943" alt="图片8" src="https://github.com/duanruixia/duanDataMining/assets/167868610/b9f2beab-8f05-4f2a-bb0f-3317ef8afe40">

<img width="930" alt="图片9" src="https://github.com/duanruixia/duanDataMining/assets/167868610/0f7f13a8-5c33-4e7e-ab7f-b4d4f0653bb1">


# 4.我想学习或获得的计算机技能

## 4.1TextCNN

最近所看的论文中有几篇都提到了TextCNN，也就通过卷积操作来捕捉文本中的局部特征，并将这些特写特征组合成全局的表示。以下是我学到的关于TextCNN所学到的基础知识。TextCNN是一种卷积神经网络，用于文本分类和其他的自然语言处理任务。

![图片10](https://github.com/duanruixia/duanDataMining/assets/167868610/fc8bafcb-d66e-470b-bed6-cf58b6f95915)


Embedding Layer：首先，文本需要被表示成计算机可以理解的形式。通常，我们使用词嵌入 (word embedding) 来将每个单词映射到一个实数向量。这个映射可以是一个预先训练好的词嵌入矩阵，也可以是模型的参数之一。上图中，"I like this movie very much!" 一句话中的每个单词和标点符号都被表示为一个长度为5的一维向量，然后拼接在一起形成这句话的 feature map。在 TextCNN 中，Embedding 层通常使用预先训练好的词嵌入 (word embedding) 进行初始化。词嵌入是一种将每个单词映射到一个实数向量的技术，它可以将自然语言转化为计算机可以处理的形式。预训练的词嵌入通常是使用大型语料库和词向量训练算法（例如 Word2Vec、GloVe 等）在无监督的情况下生成的。这些算法使用文本上下文的信息来学习每个单词的嵌入向量，使得相似的单词在向量空间中距离更近。在使用预训练词嵌入时，我们需要将每个单词映射到它对应的嵌入向量。通常，我们可以使用一个词嵌入矩阵来存储所有单词的嵌入向量。对于输入文本中的每个单词，我们可以查找对应的嵌入向量，并将其作为卷积层的输入。

![图片11](https://github.com/duanruixia/duanDataMining/assets/167868610/61d11858-97da-4fef-a07a-b7a1a26bfb1a)


Convolution Layer：接下来，我们将使用卷积层来捕捉文本中的局部特征。卷积层类似于图像处理中的卷积操作，但是它将卷积核应用于文本中的每个可能的子序列。因此，卷积层可以捕获文本中的 n-gram 特征。n-gram 是自然语言处理中常用的一种文本表示方法。它指的是将文本中的连续 n 个单词（或字符）作为一个单元进行处理。通过 n-gram，我们可以将文本转化为一个由单元序列组成的向量空间表示。这种表示方法通常用于文本分类、信息检索和语言模型等任务中。在文本分类任务中，我们可以使用 n-gram 表示文本的局部特征，并将这些特征输入到分类器中进行分类。在语言模型中，n-gram 可以用来计算单词序列的概率，并预测下一个单词的可能性。需要注意的是，n-gram 中的 n 可以是任意正整数。通常，当 n 较小时，n-gram 可以捕捉到单词之间的局部关系，而当 n 较大时，n-gram 可以捕捉到更长的文本结构。但是，当 n 太大时，将会导致维度爆炸和数据稀疏问题，影响模型的效果。上述图中不同的颜色代表不同的卷积核，也就是用来提取不同的特征。


![图片12](https://github.com/duanruixia/duanDataMining/assets/167868610/8be020b8-8e78-4f7c-b010-f6ab8902222a)

MaxPooling Layer：在卷积层之后，使用池化层来减小特征向量的维度。常见的池化操作是最大池化 (max pooling)，它返回每个特征向量中的最大值。这样做可以将每个卷积核提取的局部特征压缩成一个固定长度的向量。

![图片13](https://github.com/duanruixia/duanDataMining/assets/167868610/b17e4504-53d4-4ad6-9f32-3ae45d875f78)


Fully Connected Layer：最后，将池化后的特征向量拼接起来，并通过一个或多个全连接层来生成最终的分类结果。全连接层的作用是将不同的特征向量组合成更高层次的表示，并将它们映射到输出类别。以上便是这个模型的基础框架。

依赖解析器：dependency parsing：通过分析句子内词之间依存关系，揭示其语法结构的任务。一个句子里面两两词汇的关系，它在乎的是两个词汇间有没有关系，是什么样的关系。所得到的这种依赖关系常用来用作词与词之间的关系矩阵，作为卷积核取提取局部的文本特征。

![图片14](https://github.com/duanruixia/duanDataMining/assets/167868610/373f3cc9-d5b2-4beb-8d5b-4720d79d6626)


## 4.2记录了有关损失函数中超参数的理解
![图片15](https://github.com/duanruixia/duanDataMining/assets/167868610/d668422b-077c-476f-9ce8-482af3371555)
![图片16](https://github.com/duanruixia/duanDataMining/assets/167868610/cecfc294-ab47-44ae-ad22-782b5181457d)

![图片17](https://github.com/duanruixia/duanDataMining/assets/167868610/f4f1ff15-31ac-40a4-ae80-2525554c2751)
