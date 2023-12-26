## **Toxic Content Detection in online social networks: a new dataset from Brazilian Reddit Communities**

This is new dataset of 2,500 manually annotated examples of comments extracted from the top 10 largest Brazilian subreddits on Reddit. The dataset has been annotated by crowd-sourcing efforts with contributions from the departments of computer science (DCC) and the linguistic group of UFMG. As part of our contribution to the toxicity automatic detection and moderation of online social networks, we're making the dataset public for research.

### Dataset

The dataset contains 2,500 manually annotated comments from the most popular brazilian communities on Reddit. The data sampling proccess was a stratified sampling the number of generated publications by subreddit and the month of publication. The list of communities collected is presented below. The collected data period ranges from January 2022 to December 2022.

|   **Subreddit**  	| **Posts** 	| **Comments** 	|
|:----------------:	|:---------:	|:------------:	|
|     r/brasil     	|   110,829 	|   2,136,866  	|
|    r/desabafos   	|   115,876 	|   1,211,643  	|
|     r/futebol    	|    35,826 	|   1,214,412  	|
|    r/saopaulo    	|     7,308 	|      81,969  	|
|     r/eu\_nvr    	|    12,631 	|     188,620  	|
| r/botecodoreddit 	|     7,059 	|      57,298  	|
|    r/conversas   	|    21,967 	|     326,061  	|
|  r/investimentos 	|     9,756 	|     141,823  	|
|    r/tiodopave   	|     2,371 	|      11,584  	|
|   r/brasilivre   	|    67,301 	|    1,219265  	|
|       Total      	|   390,924 	|    6,589,541 	|


##### Annotation proccess

The annotators were divided into groups of raters and each group received a batch of comments to label. The raters were then asked to label a comment as `Toxic`, `Non-toxic`, `I do not know` and `Missing info`. During the annotation process, the labellers were encouraged to assign one of the uncertain labels when they're not sure about the toxicity of a comment or the context is missing. 

##### Available data
The dataset is available as `csv` file on the path `dataset/toxicity_br_labeled_data.csv`. The final label was assigned as a majority vote among the raters. 

### Usage
Toxicity classification models are very scarce for low-resource languages such as Brazilian Portuguese. The goal of this dataset is to foster the experimentation and advancement of applied Machine Learnign techiniques in order to improve existing methods as well as propose new ones. For instance, one can train and benchmark with existing machine learning models from scratch. Also, another alternative is to fine-tune existing large language models.

More details about the methology and data characterization can be found on the published paper.

### Citation
This work can be cited in the following bibitex format.


```bibitex
@inproceedings{},
  title={Toxic Content Detection in online social networks: a new dataset from Brazilian Reddit Communities},
  author={},
  booktitle={},
  pages={},
  year={2024}
}
```

### License
This dataset is available under the MIT license and is free to use for personal and research purposes. Learn more on the license page.
