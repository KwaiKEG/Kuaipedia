# Data Intruction

To download the full subset and experimental results of Kuaipedia, please use the following link: 

> link: https://pan.baidu.com/s/1yUB97aL2rBVt-Q0c6sYIcw code: kwyw

If you're experiencing any issues with downloading the data file, please don't hesitate to reach out to myscarletpan@gmail.com for assistance.

## Videos
| Field           | Description                                    | Example                                                                                                                              |
|-----------------|------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------|
| video_id        | video ID, which can link to the video on https://www.kuaishou.com/                                   | [3xa9yb9c4bxima6](https://www.kuaishou.com/short-video/3xa9yb9c4bxima6)                                                                                                                    |
| video_title     | The title on the cover                                    | 高级扦插玫瑰                                                                                                                       |
| video_caption   | The user-edit caption                                       | #玫瑰 #扦插 #扦插玫瑰花 15天就能生根了，还有不会的私信我                                                                                 |
| video_ocr       | OCR results                                        | 高级扦插玫瑰  哥贝  扦插玫瑰花 在土豆上  插进土豆里  养护三天浇 有喜欢养花花                              |
| video_asr       | ASR results                                      | 给大家分享一个添插玫瑰花的技术，首先我们要找到这种无病虫害的枝条。 在土豆上打一个洞，把枝条剪下来，插进土豆里，然后再将土豆埋进去。 00:00:12 这些都做完以后，把花放在通风散光的地方。养腹三天浇一次水即可，15天玫瑰花就可以生根了，有喜欢养花的朋友可以点赞关注，每天分享养花知识。                                            |
| video_summary   | Summary by GPT | 这个视频介绍了一种添插玫瑰花的技术，需要找到无病虫害的枝条，将其插入土豆中，再将土豆埋入土壤中，放在通风散光的地方，每三天浇一次水，15天后玫瑰花就可以生根。建议喜欢养花的人关注该频道，获取更多养花知识。 |
| video_rank      | The position under an aspect                           | 1                                                                                                                                  |
| item_title      | The title of item                                         | 玫瑰                                                                                                                               |
| item_subtitle   | The subtitle of item                                     | 蔷薇科蔷薇属多种花卉通称                                                                                                           |
| aspect_name     | The aspect                                     | 扦插                                                                                                                               |
| score           | The score                                      | 0.7417990367666271                                                                                                                 |


## Items
| Field           | Description                                    | Example         |
|-----------------|------------------------------------------------|-------------------------------------------------------------------|  
| title | the title of the item |	玫瑰 |
| subtitle | the subtitle/navigation of the item | 蔷薇科蔷薇属多种花卉通称 |
| synonyms | title synonyms | 野玫瑰/玫 瑰/玫瑰/玫瑰花 |
| baike_url | link to baidubaike | https://baike.baidu.com/item/%E7%8E%AB%E7%91%B0/63206 |
| wiki_url | link to wikipedia | https://zh.wikipedia.org/wiki/%E7%8E%AB%E7%91%B0 |
| aspect_list | list of aspects | [{"name": "主要种类", "level": 1} , ...]|
