# 👻 Face Swaper built by Eric Bai

## Face Swaper Ethics 

In this study, we propose a new one-shot pipeline for image-to-image and image-to-video face swap solutions - GHOST (Generative High-fidelity One Shot Transfer). Deep fake synthesis methods have been improved a lot in quality in recent years. The research solutions were wrapped in easy-to-use API, software and different plugins for people with a little technical knowledge. As a result, almost anyone is able to make a deepfake image or video by just doing a short list of simple operations. At the same time, a lot of people with malicious intent are able to use this technology in order to produce harmful content. High distribution of such a content over the web leads to caution, disfavor and other negative feedback to deepfake synthesis or face swap research.


## Image Swap Results 
![](/examples/images/example1.png)

![](/examples/images/example2.png)


### Tips
  1. For the first epochs we suggest not to use eye detection loss and scheduler if you train from scratch.
  2. In case of finetuning you can variate losses coefficients to make the output look similar to the source identity, or vice versa, to save features and attributes of target face.
  3. You can change the backbone of the attribute encoder and num_blocks of AAD ResBlk using parameters `--backbone` and `--num_blocks`.
  4. During the finetuning stage you can use our pretrain weights for generator and discriminator that are located in `weights` folder. We provide the weights for models with U-Net backbone and 1-3 blocks in AAD ResBlk. The main model architecture contains 2 blocks in AAD ResBlk.
  
## Cite
If you use our model in your research, we would appreciate using the following citation

Thank you.
Eric Bai
