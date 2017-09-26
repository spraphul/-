---
layout: post
section-type: post
title: Using Transfer Learning
category: Deep Learning
tags: [ 'tutorial' ]
---


To explain this, let us take the example of Inception-v3(an image classifying model), developed by Google.
This model has been trained on a huge dataset of images(Imagenet) which consists more than a million images 
of over 1000 classes. Now to make a model which classifies a dataset in some set of labels requires training over 
a large set of data specially when you are using deep learning algorithms. Training such a large data is not very economical 
in terms of time and space. It requires CPUs with large memory or good GPUs like NVIDIA(GEFORCE), TITAN X etc. Now, even if you 
train your data on these, it will take hours to train and if the data is of order of millions, weeks of time is taken.
Here transfer learning comes into play. According to wikipeda, " Transfer learning or inductive transfer is a research problem in machine learning that focuses on storing knowledge gained while solving one problem and applying it to a different but related problem." Instead of learning the weights from randomly initialised values, we initialise them to the values learnt by a standard model like Inception-v3.

### Retraining Inception-v3 for our own dataset

First Step is to Prepare the dataset
<pre><code data-trim class="yaml">
-Download the dataset for the labels you want to classify.
-Keep the images of each label in a separate folder and give the folder a name same as the label.
-Put all the folders in a single folder and name it.
-That's it, you have prepared your datset.
</code></pre>

<pre><code data-trim class="c">
{% raw %}
int main()
{
  printf("Hello, world of syntax highlighting!");

  return 0;
}
{% endraw %}
</code></pre>

<small>If you don't need syntax highlight in your website you can disable it by setting the syntax-highlight variable to False</small>

