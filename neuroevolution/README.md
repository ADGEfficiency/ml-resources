[Deep Neuroevolution of Self-Interpretable Agents](https://attentionagent.github.io/)

[Computers Evolve a New Path Toward Human Intelligence | Quanta Magazine](https://www.quantamagazine.org/computers-evolve-a-new-path-toward-human-intelligence-20191106)

Instead of hard-coding the rules of reasoning, or having computers learn to score highly on specific performance metrics, they argue, we must let a population of solutions blossom. Make them prioritize novelty or interestingness instead of the ability to walk or talk. They may discover an indirect path, a set of steppingstones, and wind up walking and talking better than if they’d sought those skills directly.

In neuroevolution, you start by assigning random values to the weights between layers. This randomness means the network won’t be very good at its job. But from this sorry state, you then create a set of random mutations — offspring neural networks with slightly different weights — and evaluate their abilities. You keep the best ones, produce more offspring, and repeat. (More advanced neuroevolution strategies will also introduce mutations in the number and arrangement of neurons and connections.) Neuroevolution is a meta-algorithm, an algorithm for designing algorithms. And eventually, the algorithms get pretty good at their job.

Instead of selecting the networks that performed best on a task, novelty search selected them for how different they were from the ones with behaviors most similar to theirs. (In Picbreeder, people rewarded interestingness. Here, as a proxy for interestingness, novelty search rewarded novelty.)

One of its biggest drawbacks, according to Risto Miikkulainen, a computer scientist at the University of Texas, Austin (and Stanley’s former doctoral adviser), is the amount of computation it requires. In traditional machine learning, as you train a neural network, it gradually gets better and better. With neuroevolution, the weights change randomly, so the network’s performance might degrade before it improves.

Another drawback is the basic fact that most people have a particular problem that they’d like to solve. A search strategy that optimizes for interestingness might get you to a creative solution for that particular problem. But it could lead you astray before it puts you on the right path.
