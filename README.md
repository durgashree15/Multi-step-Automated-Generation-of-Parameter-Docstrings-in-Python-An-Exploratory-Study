# Multi-step-Automated-Generation-of-Parameter-Docstrings-in-Python-An-Exploratory-Study

The project aims to achieve significant improvements in BLEU-4 and METEOR scores over existing generative models by engineering a cutting-edge framework to fine-tune PLMs using 111k Python functions for generating comprehensive docstrings. The developed framework produces meticulously formatted docstrings encompassing data types, descriptions, etc. Score-based and human-centered evaluations with 17 developers demonstrated the framework’s superiority in enhancing documentation quality. Pre-trained models like CodeBERT, CodeT5, UniXcoder were fine-tuned to achieve extensive descriptions while task-specific models were fit into the pipeline to include derivatives derived from taxonomies for developing detailed parameter docstrings.

#### Link to the code repository

https://tinyurl.com/2p8wpe49

#### Full publication can be accessed at 

https://arxiv.org/pdf/2311.06453

https://dl.acm.org/doi/abs/10.1145/3639478.3643110

<div align = "center">
  <p> Data Preprocessing for extentive parameter-wise docstring ggeneration</p>
  <img src="https://github.com/user-attachments/assets/6b9775f7-e160-4784-ac27-98033ffa071a" alt="Sample Image" width="500" height="350">
</div>

<div align = "center">
  <p>The pipeline for our proposed multi-step approach</p>
  <img src="https://github.com/user-attachments/assets/6585c873-5b9e-4cc2-9326-3ab138fd09a5" alt="Sample Image" width="700" height="350">
</div>

<div align = "center">
  <p> Docstrings generated from the multi-step pipeline</p>
  <img src="https://github.com/user-attachments/assets/53e799f3-a572-4052-a7de-8026018cbf32" alt="Sample Image" width="500" height="350">
</div>

#### Summary of the work done
1. Models fine-tuned on code structures to produce descriptions for parameter docstrings were not consistent in the number of technical details included. Therefore, we combined the outputs from task-specific models to ensure the inclusion of the different technical directives of a parameter along with the description.

2. Detailed docstring generation is ill-modelled as a fully generative task. Owing to an overwhelming amount of documentation debt, the quality of training data is not good enough to enable generative models to learn to include all crucial documentation directives. The difference in the underlying nature of tasks required to generate each directive of the docstring adds to the complexity. Therefore, a combination of multiple models adept at generating each directive is a more reliable approach to generating detailed docstrings.

3. Practitioners prefer the output from the multi-step approach with all the technical details over output from a single model with just a description. There is sound acceptance of our approach in terms of completeness and the technical nature of the content.


