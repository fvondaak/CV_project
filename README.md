# Representation Adaptation in Transfer Learning
Transfer learning enables deep neural networks to adapt to new tasks by reusing representations learned during pretraining, reducing the need for large labeled datasets and extensive computational resources. However, the extent to which pretrained features remain transferable across different visual domains, and how they evolve during fine-tuning, remains an active area of research. This project investigates representation learning and adaptation in pretrained computer vision models, using cross-domain image classification as an experimental setting.  
  
**The research will include:**  
Until end of November (hopefully):
- Baseline Implementation: Establish conventional transfer learning baselines using ImageNet-pretrained architectures (e.g., ResNet), including linear probing, partial fine-tuning, and full fine-tuning.
- Dataset Selection: Evaluate transfer learning on datasets with varying degrees of domain shift, including medical imaging datasets maybe even with limited labeled data and class imbalance.
- Literature Review: Investigate recent research on representation adaptation in finetuning and efficient finetuning strategies.
- Paper Reproduction: Reimplement a promising research method and evaluate its performance against established baselines under comparable experimental conditions.
- Representation Analysis: Examine internal feature representations using methods like linear probing, PCA, Centered Kernel Alignment (CKA) and other diagnostic techniques (depends on what's useful).
- Write a small little report, a markdown is probably also fine  

From December on:
- Think of hypotheses explaining observed differences in model behavior evolution of representations and generalization performance.
- Controlled Experiments & Ablation Studies: Design experiments to test these hypotheses, isolate contributing factors, and investigate the mechanisms behind
different adaptation strategies.

Stretch Goals:
- Method Extensions: Explore potential modifications or improvements to the reproduced method based on insights gained from representation analysis.
- Generalization: Investigate whether experimental findings extend to different model architectures, datasets, and levels of domain shift.


The scope remains intentionally exploratory, allowing research questions, experimental methods, and potential extensions to evolve based on empirical findings. The emphasis is on reproducible experimentation, rigorous evaluation, and hypothesis-driven analysis rather than achieving state-of-the-art classification performance.

Pretrained model sources:
ResNet-50 pretrained on imagenet-1k(torchvision): https://docs.pytorch.org/vision/main/models/generated/torchvision.models.resnet50.html  
Paper: https://arxiv.org/pdf/1512.03385  
ViT pretrained on imagenet-1k(huggingfac):  
https://huggingface.co/timm/vit_small_patch16_224.augreg_in1k  
Paper: https://arxiv.org/pdf/2010.11929  
Convnext-tiny pretrained on imagenet-1k(torchvision):  
https://docs.pytorch.org/vision/main/models/generated/torchvision.models.convnext_tiny.html?utm_source=chatgpt.com  
Paper:https://arxiv.org/pdf/2201.03545  
https://docs.pytorch.org/vision/main/models/generated/torchvision.models.convnext_tiny.html?utm_source=chatgpt.com  

