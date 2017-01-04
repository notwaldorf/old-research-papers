# academia
Before I wrote C++ and JavaScript, I did some Reinforcement Learning research. This stuff had a website, now it doesn't, so here it is, for posterity. The abstracts are
nerdy, and verbose, and I am sorry.

## Learning Predictive State Representations

Learning agents that interact with complex environments often cannot predict the exact outcome of their actions due to noisy sensors or incomplete knowledge of the world. Learning the internal representation of such partially observable environments has proven to be a difficult problem. In order to simplify this task, the agent can choose to give up building an exact model which is able to predict all possible future behaviours, and replace it with a more modest goal of predicting only specific quantities of interest. This work is primarily concerned with ways of representing the agent's state that allows it to predict the conditional probability of a restricted set of future events, given the agent's past experience. Because of memory limitations, the agent's experience must be summarized in such a way as to make these restricted predictions possible. We introduce the idea of history representations, which allow us to condition the predictions on "interesting" behaviour, and present a simple algorithmic implementation of this framework. The learned model abstracts away the unnecessary details of the agent's experience and focuses only on making certain predictions of interest. We illustrate our approach empirically in small computational examples, demonstrating the data efficiency of the algorithm.

📝 [Monica Dinculescu, _Approximate Predictive Representations of Partially Observable Systems_, M.Sc. Thesis, McGill University, 2010](./papers/thesis.pdf)

📝 [Monica Dinculescu, Doina Precup, _Approximate Predictive Representations of Partially Observable Systems_, ICML 2010](./papers/icml.pdf)

📜 [_Learning Approximate Representations of Partially Observable Systems_, MSRL, Montreal, June 2009](./posters/msrl.pdf)

## Learning approximate predictive models

State representations which rely on prior models, such as partially observable Markov decision processes (POMDPs) are computationally expensive and sensitive to the accuracy of the underlying model dynamics. Recent work by Hundt et al. proposes a duality construction that yields a minimal deterministic model which can make the same predictions about future observations as the original POMDP. We extend this theory to a class of history-based models, and consider situations in which an agent is only interested in a subset of the available observations. We show how to construct a history machine from any POMDP, and show that the double dual is well formed. Finally we propose an efficient algorithm that learns this structure from data, and is able to make predictions with the same accuracy as the original POMDP.

📝 [Summary](./papers/history.pdf)

📝 [Monica Dinculescu, Christopher Hundt, Prakash Panangaden, Joelle Pineau, Doina Precup, _The Duality of State and Observation in Probabilistic Transition Systems_, TbiLLC 2011](http://link.springer.com/chapter/10.1007%2F978-3-642-36976-6_14)

## Duality for states and observations

We study a double dual construction which gives a minimal and deterministic representation of a partially observable Markov decision process (POMDP), while retaining the same behaviour. We discuss two types of equivalence relations on states, namely linear and branching ones, and construct a hierarchy of them. Additionally, we show that bisimulation is the strongest equivalence relations on states, and that just traces of a system are not enough to capture its behaviour.

📝 [Summary](./papers/equiv.pdf)

📝 [Kripke Machines and Duality for Automata](./papers/duality.pdf)

📜 [_The Duality of State and Observations_, QEST, 2007](./posters/qest.pdf)

## Predictive algorithm for partially observable systems

Work by Still and Bialek proposes an information theoretic approach that compresses a system's available history into an internal representation and maximizes its predictive power. In order to validate the asymptotic nature of the theoretical algorithm, we present empirical results that demonstrate the accuracy of the internal representation as well as its predictive powers. In addition, we propose two alternative approaches that may ensure faster convergence times and more accurate optimal action strategies.

[S. Still, M. Dinculescu, D. Precup, An Information Theoretic Approach for Building Approximate Predictive Models, NIPS Workshop, 2006](./papers/cdmp.pdf)
