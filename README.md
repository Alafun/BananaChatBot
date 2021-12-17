# BananaChatBot
 Task for NLP(Natural Language Process) class.  
 If you love the repo or the repo is helpful for you, the star ⭐ is welcomed 🤗. </br>
 **But the repo is only to record the time about my life and happiness.🤗 Peace and love 🤟**   

  Deployment:  [ ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)   ](https://colab.research.google.com/drive/15xKwj3iOQkWaTKy6fUdbnA1w3qvlVX8t?usp=sharing) [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Alafun/BananaChatBot/HEAD)

## Quick Start

### Method 1
Click ![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg) buttom or [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Alafun/BananaChatBot/HEAD) buttom above.

### Method 2
#### Step1:
Clone this repo
#### Step2:
Run `jupyter-notebook` and open [deployment_of_chatbot.ipynb](https://github.com/Alafun/BananaChatBot/blob/main/deployment_of_chatbot.ipynb)
#### Step3:
Run code

### Method 3
Based on [Method 2](#method-2) Load `model.npz`

```py
load_weights = tl.files.load_npz(name='model.npz')
tl.files.assign_weights(load_weights, model_)
```

## File tree (partly)

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
### What
> What are you guys doing
I am inspired by my teacher, Banana, who is about the same age as us and *qt* as banana.
Although the data of today is December 17, 2021 and the time for task goes by, we will *never stop* and **keep running**.
![image](https://user-images.githubusercontent.com/78416589/146551317-ceb5491f-37c1-4904-bddf-a5a3b86d2b23.png)



<details>
<summary>PS: </summary>
<p>The links that appear in the image: </p>
<p>https://zhuanlan.zhihu.com/p/32455898</p>
<p>https://github.com/lc222/seq2seq_chatbot</p>
<p>https://github.com/lc222/seq2seq_chatbot_new</p>
</details>


### Who
### Done
- [x] Simple deployment
- [x] Simple useage
- [x] Simple show

### To DO
- [ ] Further konwledge about *Seq2seq* for me
- [ ] Better show skill for me
- [ ] Deploy on *github pages*
- [ ] Train a powerful model
- [ ] Perform well for interaction


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
