
[Uber's Synthetic Training Data Speeds Up Deep Learning by 9x - InfoQ](https://www.infoq.com/news/2020/01/uber-deep-learning-speedup/)

Generative Teaching Networks (GTN) that produces synthetic training data for neural networks which allows the networks to be trained faster than when using real data. 

GTN-neural architecture search (GTN-NAS) is competitive with the state of the art NAS approaches that achieve top performance while using orders of magnitude less computation than typical NAS methods.

## Text Books

[Understanding Deep Learning](https://udlbook.github.io/udlbook/)

[Deep Learning for Programmers](https://aiprobook.com/deep-learning-for-programmers/)

## Annotated Papers

[Annotated Research Paper Implementations](https://nn.labml.ai/)

## Graph Neural Nets

[A Gentle Introduction to Graph Neural Networks](https://distill.pub/2021/gnn-intro/)

---

[The New XOR Problem](https://blog.wtf.sg/posts/2023-02-03-the-new-xor-problem/)

[Kayzaks/HackingNeuralNetworks](https://github.com/Kayzaks/HackingNeuralNetworks) - a small course on exploiting and defending neural networks

[Gaussian Processes are Not So Fancy](https://planspace.org/20181226-gaussian_processes_are_not_so_fancy/)

[Understanding optimization in deep learning by analyzing trajectories of gradient descent](http://www.offconvex.org/2018/11/07/optimization-beyond-landscape/)

[Deep Learning Performance Cheat Sheet](https://towardsdatascience.com/deep-learning-performance-cheat-sheet-21374b9c4f45)

[Attention? Attention!](https://lilianweng.github.io/lil-log/2018/06/24/attention-attention.html)

https://www.quora.com/Can-neural-networks-have-thousands-of-output-classes

[Back-propagation, an introduction](http://www.offconvex.org/2016/12/20/backprop/)

[Introduction to Machine Learning Based AI - DeepMind](https://www.youtube.com/watch?v=iOh7QUZGyiU&list=PLqYmG7hTraZDNJre23vqCGIVpfZ_K2RZs)

[37 Reasons why your Neural Network is not working](https://blog.slavv.com/37-reasons-why-your-neural-network-is-not-working-4020854bd607)

[Yes you should understand backprop - Andrej Karpathy](https://medium.com/@karpathy/yes-you-should-understand-backprop-e2f06eab496b)

Prof. Yoshua Bengio - Deep learning & Backprop in the Brain - [youtube](https://www.youtube.com/watch?v=FhRW77rZUS8) - [review](https://github.com/ADGEfficiency/personal/blob/master/reviews/work/Bengio_backprop_brain.md)

Intro to optimization in deep learning: Busting the myth about batch normalization - [blog post](https://blog.paperspace.com/busting-the-myths-about-batch-normalization/)

Neural network implemented with light instead of electrons - [ars](https://arstechnica.com/science/2018/07/neural-network-implemented-with-light-instead-of-electrons/)

Troubleshooting Convolutional Neural Networks - [article](https://gist.github.com/zeyademam/0f60821a0d36ea44eef496633b4430fc)

[Checklist for debugging neural networks](https://towardsdatascience.com/checklist-for-debugging-neural-networks-d8b2a9434f21)

Simple model first

Overfit on single data point - 100 % accuracy

Scale of the loss is appropriate

Initial loss

[Can neural networks have thousands of output classes?](https://www.quora.com/Can-neural-networks-have-thousands-of-output-classes)

Word2vec has 3 million output classes in the commonly used GoogleNews vectors, one for each word.

When you have so many output classes, though, it becomes problematic to do things like updating billions of weights or sampling from an output probability distribution with 3 million option. There are many ways to approach this problem (see Approximating the Softmax for Learning Word Embeddings for some review by Sebastian Ruder). The original method was to use Hierarchical Softmax, which puts the output classes into a tree and then training & sampling only have to visit one path through the tree. During training, however, it is preferable to use techniques such as Noise Contrastive Estimation, which involves updating weights for only a small subset of all classes at each training step (where the updated weights support the true labeled class and a subsample of negative classes for the example being trained).

[Deep Learning optimization](https://www.reddit.com/r/MachineLearning/comments/fkurza/d_deep_learning_optimization/)

[Improved protein structure prediction using potentials from deep learning - Deep Mind](https://www.nature.com/articles/s41586-019-1923-7.epdf?author_access_token=Z_KaZKDqtKzbE7Wd5HtwI9RgN0jAjWel9jnR3ZoTv0MCcgAwHMgRx9mvLjNQdB2TlQQaa7l420UCtGo8vYQ39gg8lFWR9mAZtvsN_1PrccXfIbc6e-tGSgazNL_XdtQzn1PHfy21qdcxV7Pw-k3htw%3D%3D)

[Why Deep Learning Works Even Though It Shouldn’t – Ryan Moulton's Articles](https://moultano.wordpress.com/2020/10/18/why-deep-learning-works-even-though-it-shouldnt/)

There’s a good set of params somewhere nearby.

When we start walking to it, we can’t ever get stuck along the way, because there are no local optima.

In the classical regime, once we’ve stumbled upon a good set of parameters, we’ll know it and we can just stop.

In the double descent regime, once we’ve stumbled upon a good set of parameters for the lower layers, gradient descent will tend to find an average of all the good models in the higher layers.

---

An optimization algorithm is best thought of as a priority queue of things to learn, and the thing that’s important to prove is that your algorithm learns the good things first. When your model peaks on the validation set, it is starting to learn more bad things than good things. When your model is reaching zero training loss in the second descent mode, it is building a random/average function out of the good things it learned early in training.

---

For me this way of thinking explains a lot of otherwise confusing phenomena, like why distillation works so well. Distillation causes the student model to learn more of the good things before it learns the bad things, because the teacher model knows more good things than bad things already. This is why it’s possible for a more powerful model to learn usefully from a weaker one.
