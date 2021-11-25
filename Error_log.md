## ModuleNotFoundError: No module named 'tensorflow.contrib'

````python
----> 7 from tensorflow.contrib.rnn import LSTMCell
````

> ```python
> ---------------------------------------------------------------------------
> ModuleNotFoundError                       Traceback (most recent call last)
> <ipython-input-5-006dda35b43a> in <module>()
>       5 import re
>       6 import tensorflow as tf
> ----> 7 from tensorflow.contrib.rnn import LSTMCell
>       8 from dynamic_seq2seq_model import dynamicSeq2seq
>       9 import jieba
> ModuleNotFoundError: No module named 'tensorflow.contrib'
> ```

参考了 [Stack Over Flow 链接](https://stackoverflow.com/questions/55082483/why-can-i-not-import-tensorflow-contrib-i-get-an-error-of-no-module-named-tenso) 原因是 `2.7.0` 不支持

```python
# from tensorflow.contrib.rnn import LSTMCell
from tensorflow.contrib import seq2seq
from tensorflow.contrib.rnn import DropoutWrapper
```

### 同遇到这个问题

- [第十章的代码中TensorFlow版本太低，很多函数不支持了，能否更新一下 ](https://github.com/nlpinaction/learning-nlp/issues/19)
- [涂大神 麻烦升级 seq2seq 程序](https://github.com/nlpinaction/learning-nlp/issues/35)

##  文件 ` seq2seq.py`缺失

原书的代码第十章 `seq2seq` 的代码，少了一个 `seq2seq.py` 文件，但是 [仓库](https://github.com/nlpinaction/learning-nlp) 里面没有，很懵。看有人提了 `issue` 但是，作者也没有回。太难了。 

### 同样还遇到了这个错误的有

- [chp10-seq2seq.py没这个文件](https://github.com/nlpinaction/learning-nlp/issues/9)
- [第十章的问答系统缺文件](https://github.com/nlpinaction/learning-nlp/issues/36)

###  解决办法

换代码，保平安 `  <| 5_5 |> 555 `

## 其他仓库

https://github.com/SysuJayce/NLP_learn

  
