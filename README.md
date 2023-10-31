# ML-Projects
---
# Machine Learning projects for my own learning and training (pun intended).

A collection of Python files and scripts and Jupyter notebooks that I have developed or I am developing, with the objective of learning and practicing various approaches, algorithms, methods and models on a varierty of Machine Learning tasks, such as Classification, Regression, Natural Language Processing, Computer Vision and more.

1. **[TEDx talk (content-based) recommender system](https://github.com/alexrodpas/ML-Projects/blob/main/TED-Talks-RecSys.ipynb)**: In this notebook, we will build a very basic content-based Machine Learning recommender system that can recommend TED talks based on the topics of your interest.
1. **[COVID 19 Detection from chest X-Rays using a CNN Classifier](https://github.com/alexrodpas/ML-Projects/blob/main/COVID19-Dtct-XRay.ipynb)**: In this notebook, we will use X-ray data of lungs from normal, COVID-positive and viral-pneumonia patients, and train a deep learning model with a Convolutional Neural Network (CNN) architecture to differentiate between them. In particular, we will fine-tune the Xception model, a deep convolutional neural network (CNN) architecture that involves [Depthwise Separable Convolutions](https://paperswithcode.com/method/depthwise-separable-convolution). This network was introduced in the paper by Francois Chollet, ["Xception: Deep Learning With Depthwise Separable Convolutions"](https://openaccess.thecvf.com/content_cvpr_2017/html/Chollet_Xception_Deep_Learning_CVPR_2017_paper.html); Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR), 2017, pp. 1251-1258.
1. **[Abstractive Text Summarization with T5 Transformer Model](https://github.com/alexrodpas/ML-Projects/blob/main/ats_t5_01.ipynb)**: Automatic summarization is one of the central problems in Natural Language Processing (NLP). Summarization consists on creating a shorter version of a document or an article that captures all the important information. It poses several challenges relating to language understanding (e.g. identifying important content) and generation (e.g. aggregating and rewording the identified content into a summary). Along with translation, it is another example of a task that can be formulated as a sequence-to-sequence task. Summarization can be *extractive* -extract the most relevant information from a document- or *abstractive* - generate new text that captures the most relevant information-. In this project we will approach the problem of single-document abstractive summarization. Following prior work, we aim to tackle this problem using the [T5 model](https://arxiv.org/abs/1910.10683). Text-to-Text Transfer Transformer (T5) is a [Transformer-based](https://arxiv.org/abs/1706.03762) model built on the encoder-decoder architecture, pretrained on a multi-task mixture of unsupervised and supervised tasks where each task is converted into a text-to-text format. We will fine-tune the pretrained T5 model on the Abstractive Summarization task using Hugging Face Transformers on the [Extreme Summarization (XSum)](https://arxiv.org/abs/1808.08745) dataset loaded from Hugging Face Datasets.
1. **[Extractive Question Answering with DistilBERT Transformer model](https://github.com/alexrodpas/ML-Projects/blob/main/extr-qa-distilBERT-01.ipynb)**. Question Answering (QA) is one of the central problems in Natural Language Processing (NLP). QA tasks return an answer given a question. Virtual assistants like Alexa, Siri or Google Assistant are examples of QA systems. There are two common types of QA tasks: **extractive** -extract the answer from the given context- and **abstractive** -generate an answer from the context that correctly answers the question. In this project we will fine-tune the DistilBERT Transformer model on the SQuAD dataset for extractive question answering., and then use this fine-tuned model for inference. The DistilBERT model was proposed in the blog post [Smaller, faster, cheaper, lighter: Introducing DistilBERT, a distilled version of BERT](https://medium.com/huggingface/distilbert-8cf3380435b5), and the paper [DistilBERT, a distilled version of BERT: smaller, faster, cheaper and lighter](https://arxiv.org/papers/1910.01108). DistilBERT is a small, fast, cheap and light Transformer model trained by distilling BERT base. It has 40% less parameters than bert-base-uncased, runs 60% faster while preserving over 95% of BERT’s performances as measured on the GLUE language understanding benchmark. We will fine-tune the DistilBERT model on the extractive QA task using the Hugging Face Transformers library and the [SQuAD dataset](https://huggingface.co/datasets/squad). The Stanford Question Answering Dataset (SQuAD) is a reading comprehension dataset, consisting of questions posed by crowdworkers on a set of Wikipedia articles, where the answer to every question is a segment of text, or span, from the corresponding reading passage, or the question might be unanswerable.
1. **[Zero-Shot Object Detection with OWL-ViT model](https://github.com/alexrodpas/ML-Projects/blob/main/ZeroShot-ObjDtct-OWL-ViT.ipynb)**. Object detection is the computer vision task of detecting instances (such as humans, buildings, or cars) in an image. Object detection models receive an image as input and output coordinates of the bounding boxes and associated labels of the detected objects. An image can contain multiple objects, each with its own bounding box and a label (e.g. it can have a car and a building), and each object can be present in different parts of an image (e.g. the image can have several cars). This task is commonly used in autonomous driving for detecting things like pedestrians, road signs, and traffic lights. Other applications include counting objects in images, image search, and more. Traditionally, models used for object detection require labeled image datasets for training, and are limited to detecting the set of classes from the training data. **Zero-shot object detection (ZSD)** is the task of object detection where no visual training data is available for some of the target object classes. In this notebook we approach the problem of Zero-shot object detection with the [OWL-ViT model](https://huggingface.co/docs/transformers/model_doc/owlvit). The OWL-ViT (short for Vision Transformer for Open-World Localization) model was proposed in [Simple Open-Vocabulary Object Detection with Vision Transformers](https://arxiv.org/abs/2205.06230) by Matthias Minderer, Alexey Gritsenko, Austin Stone, Maxim Neumann, Dirk Weissenborn, Alexey Dosovitskiy, Aravindh Mahendran, Anurag Arnab, Mostafa Dehghani, Zhuoran Shen, Xiao Wang, Xiaohua Zhai, Thomas Kipf, and Neil Houlsby. OWL-ViT is an open-vocabulary object detection network trained on a variety of (image, text) pairs. This means that it can detect objects in images based on free-text queries without the need to fine-tune the model on labeled datasets.
