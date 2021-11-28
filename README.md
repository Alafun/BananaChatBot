# BananaChatBot
 Task for NLP(Natural Language Process) class.  
 If you love the repo or the repo is helpful for you, the star ⭐ is welcomed 🤗.

  Deployment:  [ ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)   ](https://colab.research.google.com/drive/15xKwj3iOQkWaTKy6fUdbnA1w3qvlVX8t?usp=sharing)

## Quick Start

### Method 1
Click ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg) buttom above.

### Method 2
#### Step1:
Clone this repo
#### Step2:
Run `jupyter-notebook` and open [deployment_of_chatbot.ipynb](https://github.com/Alafun/BananaChatBot/blob/main/deployment_of_chatbot.ipynb)
#### Step3:
Run code

### Method 3
Based on [Method 2](## Method 2) Load `model.npz`

```py
load_weights = tl.files.load_npz(name='model.npz')
tl.files.assign_weights(load_weights, model_)
```

## File map (partly)

```shell
BananaChatBot
├─.ipynb_checkpoints
├─data
│  ├─.ipynb_checkpoints
│  ├─twitter
│  │  └─__pycache__
│  └─__pycache__
├─docs
│  ├─pic
│  └─pic2
└─support resource
```


## Intro for program

## Star

![image](https://user-images.githubusercontent.com/78416589/143778803-93db33be-e8be-4c63-b475-f95541eacf69.png)





## Ref: 

1. https://github.com/nlpinaction/learning-nlp
   1. https://github.com/nlpinaction/learning-nlp/tree/master/chapter-10/seq2seq
2. https://blog.csdn.net/daniellibin/article/details/103290169
3. http://www.lcsays.com/tags/%E8%87%AA%E5%B7%B1%E5%8A%A8%E6%89%8B%E5%81%9A%E8%81%8A%E5%A4%A9%E6%9C%BA%E5%99%A8%E4%BA%BA/
4. https://github.com/songyingxin/TextClassification
5. https://github.com/tensorlayer/seq2seq-chatbot
6. https://overreacted.io/preparing-for-tech-talk-part-1-motivation/
7. https://overreacted.io/preparing-for-tech-talk-part-2-what-why-and-how/
8. https://overreacted.io/preparing-for-tech-talk-part-3-content/
9. http://www.tlu.ee/~rajaleid/montaazh/Hero%27s%20Journey%20Arch.pdf
10. https://www.bilibili.com/video/BV1eA411u7Wj
11. https://github.com/conanhujinming/How_to_give_a_talk/blob/main/how_to_give_a_talk_conanhujinming.pdf
12. https://github.com/eternnoir/pyTelegramBotAPI
13. 《Python聊天机器人开发 基于自然语言处理与机器学习》 【印】Sumit Raj







