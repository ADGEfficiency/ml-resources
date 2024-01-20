[Mastering The New Generation of Gradient Boosting](https://towardsdatascience.com/https-medium-com-talperetz24-mastering-the-new-generation-of-gradient-boosting-db04062a7ea2) - Catboost.

[Google Brain engineer’s guide to entering the field](https://80000hours.org/articles/ml-engineering-career-transition-guide/)

[Why is machine learning 'hard'? - S. Zayd Enam](http://ai.stanford.edu/~zayd/why-is-machine-learning-hard.html)

[fast.ai course](https://course.fast.ai/)

[Google Introduction to Machine Learning](https://developers.google.com/machine-learning/crash-course/ml-intro)

[Rules of Machine Learning - Google](https://developers.google.com/machine-learning/guides/rules-of-ml/)

Blog posts

[Black-box vs. white-box models - Lars Hulstaert](https://towardsdatascience.com/machine-learning-interpretability-techniques-662c723454f3)

The accuracy vs. interpretability trade-off is based on a important assumption, namely that ‘explainability is an inherent property of the model’.
I strongly believe however that with the right ‘interpretability techniques’, any machine learning model can be made more interpretable, albeit at a complexity and cost which is higher for some models than others.

[Creating correct and capable classifiers - Ian Ozsvald](https://youtu.be/t6osKvhY6Ro?si=Dlm-N0Px4ARWdk18)

[Instrumentation, Observability & Monitoring of Machine Learning Models](https://www.infoq.com/presentations/instrumentation-observability-monitoring-ml/)

Fundamentally, what we are trying to do when we are thinking about monitoring is we're thinking about, how do we want to handle failure?

Monitoring Importance: Monitoring is crucial for understanding and managing the performance of ML models in production.

Identifying Model Failures: Models don't inherently recognize their failures or limitations, so external monitoring is essential.

One of the most important things you can do before you even remotely consider putting a model in production is to train and understand in your offline environment to see, "If I train a model using this set of features on data from six months ago, and I apply it to data that I generated today, how much worse is the model than the one that I created untrained off of data from a month ago and applied to today?" I need to understand as time goes on, how is my model getting worse? How quickly is it getting worse? At what point am I going to need to be able to replace the current model with a new one?

Models' Performance Decay: Wills noted that all models' performance degrades over time, urging regular updates and iterations.

Collaboration with Dependencies: He stressed the importance of close collaboration with teams providing inputs to the model.

Deploy Models Like Code: He advised treating model deployment similarly to code deployment, using microservices frameworks for ease.
