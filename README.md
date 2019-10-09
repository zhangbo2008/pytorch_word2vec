# pytorch_word2vec

- Recently, I am rewriting word2vec implement in c++ version and pyotrch version.

- Use pytorch to implement word2vec.

- C++ version [cw2vec && word2vec](https://github.com/bamtercelboo/cw2vec).


- Now,there are still some problems that need to be improved.

总结就是
两个单词在一句话中,位置距离在2以内,
那么就让他们的embed 后的内积取负号后作为loss
超过2的,让他们的内积加到loss里面
所以bp之后,embed的向量越近的内积大,越远的内积越小.