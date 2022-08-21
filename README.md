# Transformers Loss Landscape Exploration

In this project visualization methods of fine-tuning Transformer architecture
network on QA task were demondstrated. Visualization of the optimal state achieved
by training could be taken into consideration when setting up the
fine-tuning process.

As a result of comparing available corpora and the premise of their
creation, two datasets were selected: [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) and [Adversarial
QA](https://huggingface.co/datasets/adversarial_qa) for the QA task. 
[DistilBERT model](https://huggingface.co/distilbert-base-uncased), chosen for
significant training speed and model configuration weight advantage over
other Transformer models while not compromising accuracy, was trained on
QA task.



<p align="center">
  <img src="https://github.com/stas1f1/Transformers-Loss-Landscape/blob/main/squad%200-100%20with%20loss%20on%20total.png" width="500" title="hover text">
  <p align="center">1-Dimensional loss and F1-score plot for interpolated values.
  x=0 corresponds to untuned model, x=1 corresponds to fine-tuned model
  on SQuAD 1.1 dataset
</p>


<p align="center">
  <img src="https://github.com/stas1f1/Transformers-Loss-Landscape/blob/main/heatmap_final.png" width="500" title="hover text">
  <p align="center">2-Dimensional loss surface contour plot. (0,0) point
  corresponds to untuned model, (0,1) point corresponds to fine-tuned model
  on SQuAD 1.1 dataset

</p>

<p align="center">
  <img src="https://github.com/stas1f1/Transformers-Loss-Landscape/blob/main/heatmap_trajectory_final.png" width="500" title="hover text">
  <p align="center">Visualization of projected optimization trajectory on
  2-dimensional loss surface contour plot. (0,0) point corresponds to untuned
  model, (0,1) point corresponds to fine-tuned model on SQuAD 1.1 dataset

</p>

Work based on:
> Hao Li, Zheng Xu, Gavin Taylor, Christoph Studer and Tom Goldstein. [Visualizing the Loss Landscape of Neural Nets.](https://arxiv.org/pdf/1712.09913.pdf) NIPS, 2018.

Made with Python as a part of thesis for masters, FDT ITMO
