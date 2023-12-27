## **Toxic Content Detection in online social networks: a new dataset from Brazilian Reddit Communities**

This work was accepted by the 16th International Conference on Computational Processing of Portuguese (PROPOR 2024). The paper proposes a new dataset of 2,500 manually annotated examples of comments extracted from the top 10 largest Brazilian subreddits on Reddit. The dataset has been annotated by crowd-sourcing efforts with contributions from the departments of computer science (DCC) and the linguistic group @ UFMG. As part of our contribution to the toxicity automatic detection and moderation of online social networks, we're making the dataset public for research.

### Dataset

The dataset contains 2,500 manually annotated comments from the most popular brazilian communities on Reddit. The data sampling proccess was a stratified sampling by the number of generated publications by subreddit and the month of publication. The list of communities collected is presented below. The collected data period ranges from January 2022 to December 2022.

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

Table 1 - Posts and comments by subreddit for the period of 2022-01 to 2022-12.

##### Annotation proccess

The annotators were divided into groups of raters and each group was assigned a batch of comments to label. The raters were then asked to label a comment as `Toxic`, `Non-toxic`, `I do not know` and `Missing info`. During the annotation process, the raters were encouraged to assign one of the uncertain labels when they're not sure about the toxicity of a comment or the context is missing. 

##### Available data
The dataset is available as `csv` file on the path `dataset/toxicity_br_labeled_data.csv`. The final label was assigned as a majority vote among the raters. The available data are the original collected comment `ID` and `body`. The label was created from the original classification from the annotators. No data processing has been done on this version of the dataset. The overall `schema` of the dataset if presented below.

- `id`: The unique identifier of the comment on the Reddit platform
- `body`: The original comment text publication
- `is_toxic`: The final label of a given comment. The label is `0` for non-toxic comments, `1` for toxic comments and `-1` for comments where the raters disagreed about the toxicity

### Usage
Toxicity classification models are very scarce for low-resource languages such as Brazilian Portuguese. The goal of this dataset is to foster the experimentation and advancement of applied Machine Learning techiniques in order to improve existing methods as well as propose new ones. For instance, one can train and benchmark with existing machine learning models from scratch. Also, another alternative is to fine-tune existing large language models.

More details about the methology and data characterization can be found on the published paper.

### Citation
This work can be cited in the following format.

```cite
Lima, Q. Luiz Henrique; Pagano, S. Adriana; da Silva, A.P.C. 2024. Toxic Content Detection in online social networks: a new dataset from Brazilian Reddit Communities. 16th International Conference on Computational Processing of Portuguese (PROPOR 2024).
```

### License
This dataset is available under the MIT license and is free to use for personal and research purposes. Learn more on the license page.
