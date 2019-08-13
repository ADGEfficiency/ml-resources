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
