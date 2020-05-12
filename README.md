# Technical Nuances of World of Deep-Learning | Reinforcement-Learning | Deep-Reinforcement-Learning
In this repository, sharing 

 - ["AI Code Applications"](#deepNN-apps) for 
    * **Jupyter notebook (interactive python notebook/ .ipynb)** for code samples in Deep Learning/ Deep Reinforcement Learning/ Recommendation engine. 
    * Real code as well as pseudocode
    * **Docker**, dockerfiles, docker run
    * **Microservice (rather micro web framework)** for deploying AI models as **AI-as-a-Service**
 - [FAQ on DL/ML/AI (Interview questions list)](README_FAQ_Interview_DL_ML_AI.md)
 - [Taxonomy of Audio & Speech processing domain](README_Taxonomy%20of%20Speech%20%26%20Audio%20domain.md)
 - [Python advanced concepts (such as Python_@class_@static_methods_WebCrawler_RESTfulAPI_TimeComplexity et al)](README_CorePython_AdvancedOperations.md)
 - [Hyper Parameter Optimization (HPO) in Classical ML - Grid Serach/Random Search](README_Grid_Random_Search_HyperParameterOptimization.md)
 - [Infographics as Cheatsheet](Infographics)
 - [Additional references for learning and career transitioning to the world of 'DL,RL,DRL,NLP,ML,OCR'](#refernce)
 

# Deep Learning application with latest architectures and models
Deep Learning applications that leverage latest architectures and models 


Deep Learning Applications 
---------
<a name="deepNN-apps"></a>

Please refer to following folders to go through the 
          **interatcive IPYNB** files for the following Deep Learning **Computer Vision AI Models** , along with related **dockers & docker run time commands** for the models, and also detailed refernce blogs from MEDIUM.
          
- **[Automated Number Plate Detection- Computer Vision model](anpr)** - Number plate detection with Supervisely and Tensorflow [(medium)](https://medium.com/p/e84c74d4382c)

- **[Image Segmentation- Computer Vision model](unet_training)** - Training road scene segmentation on Cityscapes with Tensorflow and UNet [(medium)](https://medium.com/p/1232314781a8)

- **[Object Detection- Computer Vision model](ssd)** - Combining Cityscapes and Mapillary to train SSD using Supervise.ly 

- **[Custom OCR Engine/Model- Computer Vision model](anpr_ocr)** - Plane number recognition with Keras [(medium)](https://hackernoon.com/latest-deep-learning-ocr-with-keras-and-supervisely-in-15-minutes-34aecd630ed8)

- **[flask_apps for creating AI-as-a-Service](flask_apps)** - Using Flask Micro web framework to create Predict RESTful API service (AI-as-a-Service) 

Prerequisites for DL Applications
-------------
- **Docker - Highly recommended** 

   *[Dockerfile, docker build, nvidia-docker run for anpr](anpr/docker)

   *[Dockerfile, docker build, nvidia-docker run for anpr_ocr](anpr_ocr/docker)

   *[Dockerfile, docker build, nvidia-docker run for ssd](ssd/docker)

   *[Dockerfile, docker build, nvidia-docker run for unet_training](unet_training/docker)

- **CUDA-capable GPU is required for training**
- An account on [Supervise.ly](https://supervise.ly) for data annotation
- **Microservice for AI Model binary deployment as AI-as-a-Service**
    [flask_apps for creating AI-as-a-Service](flask_apps)  Using Flask Micro web framework to create Predict RESTful API service (AI-as-a-Service) 


Additional reference for DL
---------------------------

https://github.com/llSourcell/Learn_Deep_Learning_in_6_Weeks/

https://www.analyticsvidhya.com/blog/2017/05/25-must-know-terms-concepts-for-beginners-in-deep-learning/

http://deeplearning.stanford.edu/tutorial/



# Deep REINFORCEMENT Learning application Reference with latest architectures and models  

**RL/DRL**
-----------

https://skymind.ai/wiki/deep-reinforcement-learning

https://www.analyticsvidhya.com/blog/2017/01/introduction-to-reinforcement-learning-implementation/

https://towardsdatascience.com/applications-of-reinforcement-learning-in-real-world-1a94955bcd12

<a href="https://www.youtube.com/watch?v=2pWv7GOvuf0"><img src="https://thumbs.gfycat.com/GreedyLeadingAnophelesmosquito-max-1mb.gif" width="240" height="180" border="10"/></a> ([Click on the Image link](https://www.youtube.com/watch?v=2pWv7GOvuf0) for "Video Lecture by David Silver on Reinforcement-Learning")

<a name= "refernce"></a>
# Additional Reference for NLP/Classical ML/OCR etc

### NLP application reference

https://medium.com/dair-ai/deep-learning-for-nlp-an-overview-of-recent-trends-d0d8f40a776d

<a href="https://www.youtube.com/watch?v=RP3tZFcC2e8&list=PL613dYIGMXoZBtZhbyiBqb0QtgK6oJbpm"><img src="https://sknadig.me/assets/posts/att_basics/att_basic.gif" width="240" height="180" border="10"/></a> 'Click on the Iamge for Video Series on Deep learning series for NLP'



### Classical ML application reference

https://skymind.ai/wiki/machine-learning-algorithms

https://towardsdatascience.com/building-a-logistic-regression-in-python-step-by-step-becd4d56c9c8




