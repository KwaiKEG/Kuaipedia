<p align="center">
<img width="256px" src="./images/logo.jpeg"/>
</p>

<p align="center">
🤗 <a href="https://huggingface.co/datasets/kwaikeg/kuaipedia" target="_blank">Dataset</a> • 📃 <a href="https://arxiv.org/abs/2211.00732" target="_blank">Paper</a>
</p>
<hr/>

**Kuaipedia** is developed by Knowledge Engineering Group in Kuaishou [(KwaiKEG)](https://github.com/KwaiKEG), collaborating with HIT and HKUST. It is the world's first large-scale multi-modal short-video encyclopedia where the primitive units are items, aspects, and short videos. 

![demo](./images/demo-case.gif)

* **Items** is a set of entities and concepts, such as [Shiba Inu](https://en.wikipedia.org/wiki/Shiba_Inu), [Moon](https://en.wikipedia.org/wiki/Moon) and [Galileo Galilei](https://en.wikipedia.org/wiki/Galileo_Galilei), which can be edited at one Wikipedia page. An item may have a title, a subtitle, a summary, attributes, and other detailed information of the item.
* **Aspects** is a set of keywords or keyphrases attached to items. Those keywords are used to describe specific aspects of the item. For example, "selection", "food-protecting", "color" of item [Shiba Inu](https://en.wikipedia.org/wiki/Shiba_Inu), or "formation", "surface conditions", "how-to-draw" of item [Moon](https://en.wikipedia.org/wiki/Moon).
* **Videos** is a set of short-videos whose duration may not exceed 5 minutes. In this paper, we only focus on knowledge videos we detected, Where we follow OECD to define knowledge as:
    * *Know-what* refers to knowledge about facts. E.g. How many people live in New York? 
    * *Know-why* refers to scientific knowledge of the principles and laws of nature. E.g. Why does the earth revolve around the sun?
    * *Know-how* refers to skills or the capability to do something. E.g. How to cook bacon in the oven.

Please refer to the paper for more details.

Kuaipedia: a Large-scale Multi-modal Short-video Encyclopedia [[Manuscript]](https://arxiv.org/abs/2211.00732)


## News
* 2023.06 - Release a subset of [[data]](#data)
* 2022.11 - 业界首个！快手提出亿级别多模态短视频百科体系快知 (The first! Kuaishou proposed a large-scale multi-modal short-video encyclopedia "Kuaipeida") [[机器之心]](https://mp.weixin.qq.com/s/_ngcmULg9-FwZER-Jlljvg)[[澎湃]](https://www.thepaper.cn/newsDetail_forward_20618591) [[知乎]](https://zhuanlan.zhihu.com/p/580890046) [[CSDN]](https://www.csdn.net/article/2022-11-07/127733976)[[51CTO]](https://www.51cto.com/article/722206.html) [[IT之家]](https://www.ithome.com/0/651/810.htm)
* 2022.08 - Obtain **"Outstanding Project Award"** in Kuaishou AI Day. 

## Data

We are excited to release a subset of Kuaipedia, featuring the most popular wiki entries for enhanced research opportunities. Along with this, we've also shared our experimental findings. Sample files can be located in the `./data` folder, accompanied by a `README.md` file to clarify each field.

To download the full subset and experimental results of Kuaipedia, please go ahead to [huggingface/dataset/kuaipedia](https://huggingface.co/datasets/kwaikeg/kuaipedia), or use the following link: 

> link: https://pan.baidu.com/s/1yUB97aL2rBVt-Q0c6sYIcw code: kwyw

The raw video can be found by concatenating `video_id` with the prefix `kuaishou.com/short-video`.  E.g. [kuaishou.com/short-video/3xwwuqndapzs6nu](https://www.kuaishou.com/short-video/3xwwuqndapzs6nu).

If you're experiencing any issues with downloading the data file, please don't hesitate to reach out to myscarletpan@gmail.com for assistance.

**Statistics**

|            | Full Dump       | Subset Dump |
|------------|-----------------|-------------|
| #Items     | > 26 million    | 51,702      |
| #Aspects   | > 2.5 million   | 1,074,539   |
| #Videos    | > 200 million   | 769,096     |

The comparative results with the baseline models are as follows:
 
|  Model   | Item P  | Item R | Item-Aspect P | Item-Aspect R | 
|  ----  | ----  |  ----  |  ----  |  ----  | 
| Random  | 87.7 | 49.8 | 36.4 | 49.6 | 
| LR  | 90.4 | 68.3 | 55.1 | 2.7 | 
| T5-small  | 93.7 | 76.1 | 79.3 | 58.5 | 
| BERT-base  | 94.3 | 77.8 | 81.5 | 62.7 | 
| GPT-3.5  | 90.5 | 86.4 | 41.8 | 95.7 | 
| Ours  | 94.7 | 79.7 | 83.0 | 65.7 | 

Feel free to explore and utilize this valuable dataset for your research and projects.

## Reference
```
@article{Kuaipedia22,
  author    = {Haojie Pan and
               Yuzhou Zhang and
               Zepeng Zhai and
               Ruiji Fu and
               Ming Liu and
               Yangqiu Song and
               Zhongyuan Wang and
               Bing Qin
               },
  title     = {{Kuaipedia:} a Large-scale Multi-modal Short-video Encyclopedia},
  journal   = {CoRR},
  volume    = {abs/2211.00732},
  year      = {2022}
}
```


## Acknowledgment

Except for the contributers to the paper. We also appreciate efforts and helps from Jingrun Zhang, Yuelei Li, Lijun Mei, Chunguang Pan, Xing Hu, Lingyu Zou, Yang Li, Dexing Yang, Wenzheng Zhao, Guixin Qiu, Lin Yang, Meijuan Yang, Teng Tu, Xinyi Zheng, Yunhui Guo and others who contributes to this project.

## Contact Us

If you are insterested in Kuaipedia and more cases, please contact us by e-mail myscarletpan@gmail.com

