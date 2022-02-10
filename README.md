# Automatic-Stance-And-Ideology-Detection-SERPs
In this repo, we tried to apply the hierarchical stance detection methodology proposed in Zhang et. al. (2019)
to obtain the stance labels of web page documents (SERPs).

In this way, our main aim was to extend the work in Gezici et. al. (2021) in which we used crowdlabels for the top-10
SERPs analysis. Owing to the automatic stance detection, we could also investigate the source of bias - if the search bias comes from
the data or algorithm.

1. We directly applied the proposed hierarchical deep learning architecture for stance detection to our problem.
2. Then, we extended the presented approach by using BERT-based features instead of handcrafted features.
3. Additionally, we also tried to incorporate "ideology information" of the documents to be able to label a given document with a stance as well as an ideology label. These two labels can be used in our stance and ideological bias analysis (Gezici et. al., 2021). 
4. Since, we could not obtain satisfactoy results - probably because our dataset that was used for fine-tuning was not large enough. Thus, we also implemented some ideas to improve the results:

  - Mixout - regularisation idea inspired by dropout,
  - LM Fine Tuning - finetuning the model on SERP domain first
