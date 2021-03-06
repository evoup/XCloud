# Content-based Image Retrieval System
## Introduction
Exploring deep metric learning & hash methods to build efficient visual search system.

**Note:** If you need an online web-based annotation tool for _Image Retrieval/ReID_, please feel free to use [CbirAnnoTool](https://github.com/lucasxlu/CbirAnnoTool.git).

![index](https://raw.githubusercontent.com/lucasxlu/CbirAnnoTool/master/index.png)

### Backbone
| Architecture | Supervision | Status |
| :---: |:---: |:---: |
| DenseNet121 | Softmax | [YES] |
| DenseNet121 | CenterLoss | [YES] |
| DenseNet121 | A-Softmax | [YES] |
| DenseNet121 | ArcLoss | [YES] |
| ResNeXt50 | A-Softmax | [TODO] |
| SeResNeXt50 | A-Softmax | [TODO] |


### Dependency
 * [Faiss](https://github.com/facebookresearch/faiss.git)
 * [Django](https://www.djangoproject.com/)
 

## About New Categories
In image retrieval and ReID tasks, how to automatically mine new categories online remains a quite challenging problem.
I propose a novel method by utilizing unsupervised learning algorithms (such as clustering) to assign pseudo label to a cluster.
After cleaning noise samples in each cluster, you can upgrade your embedding model and gallery. You can find this method implementation in [clustering.py](./clustering.py).


## License
[MIT](./LICENSE)
