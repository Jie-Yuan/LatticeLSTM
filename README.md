[Chinese NER Using Lattice LSTM][666]
====

Lattice LSTM for Chinese NER. Character based LSTM with Lattice embeddings as input.

Models and results can be found at our ACL 2018 paper [Chinese NER Using Lattice LSTM](https://arxiv.org/pdf/1805.02023.pdf). It achieves 93.18% F1-value on MSRA dataset, which is the state-of-the-art result on Chinese NER task.

Details will be updated soon.

Requirement:
======
	Python: 2.7   
	PyTorch: 0.3

Input format:
======
CoNLL format (prefer BIOES tag scheme), with each character its label for one line. Sentences are splited with a null line.

	美	B-LOC
	国	E-LOC
	的	O
	华	B-PER
	莱	I-PER
	士	E-PER

	我	O
	跟	O
	他	O
	谈	O
	笑	O
	风	O
	生	O 

Pretrained Embeddings:
====
The pretrained character and word embeddings are the same with the embeddings in the baseline of [RichWordSegmentor](https://github.com/jiesutd/RichWordSegmentor)

Character embeddings: [gigaword_chn.all.a2b.uni.ite50.vec](https://pan.baidu.com/s/1pLO6T9D)

Word(Lattice) embeddings: [ctb.50d.vec](https://pan.baidu.com/s/1pLO6T9D)


Resume NER data 
====
Crawled from the Sina Finance, it includes the resumes of senior executives from listed companies in the Chinese stock market. Details can be found in our paper.


Cite: 
========
Please cite our ACL 2018 paper:

    @article{zhang2018chinese,  
     title={Chinese NER Using Lattice LSTM},  
     author={Yue Zhang and Jie Yang},  
     booktitle={Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics (ACL)},
     year={2018}  
    }
    
---  
[666]: https://mp.weixin.qq.com/s?__biz=MzA3MzI4MjgzMw==&mid=2650744491&idx=5&sn=0f03418a0f3870a6fed319e4f00e3691&chksm=871ae2d5b06d6bc3e37d3fdd056733675626356da059c8c9b29030cdfee88cc4201374d4324d&mpshare=1&scene=1&srcid=0701DWC2WGL9kcZDNgPLJrSN#rd
