[So You Want to Study Mathematics...](https://www.susanrigetti.com/math) - if you can understand the structure of literature, if you can understand the basic grammar of the English language or any other language, then you can understand the basics of the language of the universe. 

[Foundation of Math Reading List](https://www.jmeiners.com/foundations-of-math-reading/)

[Mathematics for the adventurous self-learner](https://www.neilwithdata.com/mathematics-self-learner)

[Linear Algebra Review and Reference - 2015 - Zico Kolter (updated by Chuong Do)](http://cs229.stanford.edu/section/cs229-linalg.pdf)

[Algebra, Topology, Differential Calculus, and Optimization Theory For Computer Science and Machine Learning](https://www.cis.upenn.edu/~jean/math-deep.pdf)

[How to Read Mathematics - Shai Simonson and Fernando Gouvea](http://www.people.vcu.edu/~dcranston/490/handouts/math-read.html)

[Do software engineers need mathematics?](https://www.maa.org/external_archive/devlin/devlin_10_00.html)

Essence of linear algebra - [youtube series](https://www.youtube.com/playlist?list=PLZHQObOWTQDPD3MizzM2xVFitgF8hE_ab)

[Zico Kolter - Linear Algebra Review and Reference](http://www.cs.cmu.edu/~zkolter/course/linalg/linalg_notes.pdf)

[The Philosophy of Linear Algebra](https://sigfyg.medium.com/the-philosophy-of-linear-algebra-ac2d9ce14619)

[Algorithm Beauty of Plants](http://algorithmicbotany.org/papers/abop/abop.pdf)

[Common Errors in College Math](https://math.vanderbilt.edu/schectex/commerrs/)

[Algorithms for Decision Making - dm.pdf](https://algorithmsbook.com/files/dm.pdf)

# Intro

[Pauls Online Math Notes](https://tutorial.math.lamar.edu/) - [Calculus I](https://tutorial.math.lamar.edu/Classes/CalcI/CalcI.aspx)

[Higher Math for Beginners](https://ia801202.us.archive.org/19/items/ZeldovichYaglomHigherMathematics/Zeldovich%2C%20Yaglom%20Higher%20Math%20for%20Beginners.pdf)

My experience with learning math is that the first months are all about backtracking. You have to fill all your holes.

It's basically one big graph of concepts.

The tricky part is, most beginners simply don't know how to navigate that graph.

They see complex numbers with their exponentials and cos/sin forms and shut down.

They can learn all these concepts no problem, but finding what they need to learn defeats them. 

[Change from product to sum](https://math.stackexchange.com/questions/1336271/change-from-product-to-sum)

Sums and Products are basically interchangeable if you allow use of the logarithm because ln(𝑎⋅𝑏)=ln(𝑎)+ln(𝑏). 

If you don't know how to extend the logarithm to negative arguments, then you'll have to ensure that the product is positive and that 𝑓(𝑘) is positive.

# Bayesian

[An Overview of Bayesian Inference](https://jaydaigle.net/blog/overview-of-bayesian-inference/)

[Against Bayesianism — David Deutsch](https://josephnoelwalker.com/139-david-deutsch/)

[Introduction to Inference](https://koaning.io/posts/introduction-to-inference/)

# Stats

[NIST/SEMATECH e-Handbook of Statistical Methods](https://www.itl.nist.gov/div898/handbook/index.htm)

# Convolution

[Intuitive Guide to Convolution](https://betterexplained.com/articles/intuitive-convolution/) - [Hacker News](https://news.ycombinator.com/item?id=25190770)

# Linear Algebra

[Interactive Linear Algebra](https://textbooks.math.gatech.edu/ila/)

[Immersive Linear Algebra](https://immersivemath.com/ila/index.html)

[Why Tensors? A Beginner's Perspective](https://mfaizan.github.io/2022/03/08/why-tensors.html)

[Gilbert Strang lectures on Linear Algebra (MIT)](https://www.youtube.com/playlist?list=PL49CF3715CB9EF31D)

[On AlphaTensor’s new matrix multiplication algorithms](https://fgiesen.wordpress.com/2022/10/06/on-alphatensors-new-matrix-multiplication-algorithms/)

[AI’s compute fragmentation: what matrix multiplication teaches us](https://www.modular.com/blog/ais-compute-fragmentation-what-matrix-multiplication-teaches-us)

# ML Specific

[Mathematics for Machine Learning](https://mml-book.github.io/)

[Mathematical Introduction to Deep Learning](https://arxiv.org/abs/2310.20360)

[The Little Book of Deep Learning](https://fleuret.org/francois/lbdl.html)

[Dominance of the "Gradient Descent" over other algorithms : r/MachineLearning](https://www.reddit.com/r/MachineLearning/comments/okficy/d_dominance_of_the_gradient_descent_over_other/)

 People here stick to the "number of parameters" argument but this is not a good explanation. This is because quasi-Newton methods exist and those typically work very well in high dimensions with comparably low memory footprint.

The real reason is that we do stochastic optimization. It is already difficult to estimate the derivative of a stochastic function, but the second derivative is a lot worse. Moreover, you can't get the same benefit anymore from using second order information as in the deterministic case. As soon as the gradient is stochastic one can't do better than sub-linear convergence and the only thing to gain is better constants. 

---

Because modern neural nets have billions, if not trillions, of parameters, the Hessian matrix of billion/trillion x billion/trillion entries (which is the multivariate calculus generalization of second derivative) is simply impossible to compute or store. Second-order methods are nice but impractical, and that's also why you still see all the ongoing research in optimizing deep nets: a major theme is to find ways to (implicitly) approximate the Hessian in linear time.

---

SGD tends to select 'shallow' minima, which in turn tend to generalize better to held out data. Higher order methods may or may not have this property. 

# Textbooks

[A Programmer's Introduction to Mathematics)](https://pimbook.org/) 

[Causation, Prediction, and Search](https://www.cs.cmu.edu/afs/cs.cmu.edu/project/learn-43/lib/photoz/.g/web/.g/scottd/fullbook.pdf)

## The Matrix Cookbook - [textbook](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)

Vector norm = magnitude = length
- often used in regularization
- L1 = sum of abs values 
- L2 = square root of sum of squares
