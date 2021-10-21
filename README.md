# Hypereconomy (2021)

[![hackmd-github-sync-badge](https://hackmd.io/J1nGmV7eTB2aa38kD25ERw/badge)](https://hackmd.io/J1nGmV7eTB2aa38kD25ERw)



> [TOC]

###### tags: `research` `economy` `finance models` `math` `draft`


## Abstract

I propose novel investment model that can serve as a bridge between smart contract technology and fiat financial markets that does not yet exist.  I aimed to create business model where the value grows steadily and accordingly to its' promised and verifiable future. Economy in which liquidity is not a by-product of uncertainty, but rather the result of trust and provable stability. This concept links the acquisition of an asset directly to its curation and later, hopefully, to the solution of what is recently associated with "the identity problem".

The following ideas lay down foundations for new business models, where investments become pledges of actions that provide stability, rather than what they are now: a non-obligating acquisition based on positive estimate of numerical value commonly associated with the asset, which barely reflects its' real value.

:::info
In other words, it's a concept of markets where acquisition of an asset is accompanied by a promise/declaration of actions, which will get triggered under perfectly decidable circumstances, and their goal is to maintain the value of the asset.
:::


## The promise chains

Investment of size $v_{0}$ into $X$, comes with the promise of follow-up investment $v_{1}$, under the condition set $C$, where
$v_{0}, v_{1}$, are numerical values representing, describing size of an investment given in tradable currency.


### Example

Let's consider a startup founding round, of startup $X$, with a set of investors $I$, from which we distinguish two, investing parties, represented by $A$ and $B$, respectively. First investment is done by $A$, who invests 100,000$ in $X$, with the contract for a follow-up investment of 1,000,000$, under condition $C$, which requires someone else to invest between 100,000$ and 300,000$ within a week, that is, by the end of the investment round, during which investors, ale allowed for investing.

Follow-up contracts are automatically executed once the condition is met, execution by default is performed with the chronological order. 

:::warning
Market realisation of this concept must feature bunch of additional conditions, like time constraints, and qualifiers that will specify who is eligable, to take part in the investment round. etc. This example simply aims to illustrate the concept.
:::

## Regulating
The introduced model allows $X$ to grow indefinitely, when an upper bound staking value in each round is not set, causing the initial subject on which investors stake their money to vanish away, under the following contracts. Therefore limits must be established in order to prevent bubble growth. Those can be defined by specifying an upper bound for amount of investments, chain depth, period between rounds, or arbitrarily complicated functions that simulate possible market states, where declared contracts are challenged against all possible scenarios, thereby providing an upper bound on investment size.


## Introducing comeplete measure spaces.


Everything below might appear slight not in it's place as the initial structure of this document, got slightly distorted by the following discovery.



:::info
### Note
- _At first, my goal was to introduce only the universal measure, with standardized configuration space, along with specification of input variables. Doing what intended, led to me the pretty interesting concepts. In the near future, I'll provide tighter bounds and proper proof, for introduced concept._ 

---

### Conjecture outline
I conjecture there exist universal strategy, with the corresponding measure space, which gurantees, 0-risk follow-up investments,
where the calculated optimial market model, is an inner space product of the universal model, adjusted entirely, by parameter set, concerning prior distribution of the probability density function, which entirely conditions, the shape of the  solution space.

#### Proof outline.

Let $H(t_{0})$ denote generator of normed, measurable space with the probability density function, over the power set of conditions, and consecutive, pairs of promised actions, given as linear operators over the vector space.
 
**The target space is an interpolatate space for all $(c,λ)$ pairs, which are not defined by the market state at given timestamp**
Just for the sake of proper mathematics.

$$
  \tag H(t_{0}): P(C;λ) \rightarrow^{~F;} f(x,y)p(x,y); \forall{x,y \in \Re \rightarrow \sigma^{2} \rightarrow D^{1/2}}  \\
$$
$$
  \tag{.1} |P(C;λ)| = |2^{|C|} -1|\\
$$

- H: the transformation space, at time stamp, $t_{0}$
- P(C;$\lambda$), describes power set of conditions, with consequtive transforms. 
- $\rightarrow^{F;}$ Casting into continous space.


$$
    \tag{S(s)} 2^{n} -1 = S^2 * \Re(P_{n-2}) - (p_{x,y})
$$
where R(P...), denotes real valued n-2 dimensional vector space, being an interpolation space,
between evenly distributed function space $f(x,y)p(x,y)$, convex an continously differentiable for all 
$(x,y) \in D^{1/2}$


while $D^{1/2}$ denotes, same domains, for both continous variables, X, and Y and this is possible as this domain without loss of generality, can be derived through embedding lineary separable variables, into the the o of the variance of the probability density function, denoted as p(x,y), into the target space, evenly distributed from it's center.

I mean, such that x and y are lineary separable,

---

_This is phenomenal idea I just got_ 

All markets, with the asymptotic boundary, constraining growth of condition sets, across the founding round, such that

$$O({\sum_{n=1,2...,k} |P(C)^t_{n}| \over P(C)^t_{0}})<c $$

allow to formulate an optimal strategy model for development of investment round constraints, depending entirely on the solution of the optimization problem, of the intial values, of probablity density function, stating how likely, it is, for anyone to make an initial investment, of $v_{0}$ and the follow-up condition, such that it satifies, investment round conditions, obtained as, the solution of the mentioned problem.

### Solving with linear programming

$$maximize (P(v,C, λ); H_{0}^{\rightarrow c}H_{1}^{...n});$$
$$H_{0}^{\rightarrow ν} = H_{0}*H(vc,λ)  *maximize(H^{..n});	$$

### Convexity of the problem.

- It is convex when defined as regret minimization, where the regret function, concerns minimization of probability, that the initial investment is never done. 

- Regulation, with the respect, to the initial configuration~value distribution given by triplet, specifying first investment, doesnt seem
to be a big deal, as the adjustment can be done, by the rotation of the quaterion, across the configuraration space vector space.

:::spoiler

:::info
#### Thought archive
- It must feature, probability space, being given as the continous topo, that's in fact, interpolation space, of the power set of conditions complete condition set, locally normed, by the measurable function, locally convex and bounded.

- Am I right that 

$$
	Q(*F):\tilde= \lim_{t \rightarrow \inf}
	{F_{[t]} (\Sigma(V_t{}(A,B,...)) \over R(t)}
$$


$F$: The `function set`, I might use sometimes word `f-set`, it's pretty convinient.

$F_{[t], \phi}$: Function set accordingly discritized with the time function T.
$\phi$ is offset of the time function. This notation induces that, $\phi$ is implictly defined alongside with $F$
:::


:::warning
Real usability of the model, with bounded condition set, should become  the main subject towards further research on introduced idea.
:::

## The information game

I suppose there  might be great market potential assosiated with the idea of providing additional tradable options generated by introducing uncertainity to the information pool, that get's exposed to the investing parties concerning information on existing promises and the follow-up boundaries.


> While at first I wanted create a note, saying this will not be the subject to my main research, in the closest time:
> _"Given that, this framework, doesn't involve an investment model, which I consider at the moment, to have possitive impact on the economy (...) and I don't believe, it's already the time, for building the world, where non-deterministic things, have deterministic reason..."_
> I succeded, in convincing myself that, it might be sooner then I'd expect, till' such uncertainity becomes the only one left to humanity.

_Research of this topic should concern, knowledge problems with linear [Time function $T$](../ML/knowledge-research.md),
Game theory, with games broken down, accordingly, to the information set accessibility.
And also specify relation to existing simillar concepts, like: [futures markets](https://www.investopedia.com/terms/f/futuresexchange.asp)(I'm not sure, if my understanding of this is correct)._

## Provable trust indicators


The idea is that accurate prediction of future state of system variables can be seen as the trust indicator. 


There is smart contract with estimation of the value of the asset $X$, signed to a network at time $τ$ $Σ = E(t_{1+}, ...)$.

### Possible variants
- #### A) Estimating publicly available values. Information on estimated value is accessible by traders
    - Exact estimated value stays hidden until the time of evaluation.

- #### B) Estimating hidden variables.
    - If value of variables, shall not be revealed, it must return amortized value, with the boundaries selected proportionally, to the amount of dependent variables, size of $\Omega$  constraining inferencial capabilities of used variables, through statistical hypothesis testing, required privacy level and  overall 

Value of X, at time t gets evaluated, by given norm-measure which is immutable since the time of signing the contract to the network.
At each `evaluation timestamp`, we calculate the variance, between the real(calculated) value of $X$ and the one predicted in the signed contract.

:::success
**The calculated variance at time $t$ allows to verify the quality of an estimator and can act as provable trust-indicator.**
:::

:::info
==0~Variance proof==
Returned value in each timestamp, consist only information if variance stayed in range of $(0, ε)$, where ε is an upper bound.
:::


:::danger
It's also wrong to ever speak of trust indicators, when explicitly allowing such bidding.
:::


I see those as extandable into type of tokens, minted by marketplaces, with configuration of boundary values constraining possible configuration of the target set.
. Specified constraints draw the boundaries for estimation quality of traded assets, therefore constraining the target group and quality of
investments signable, through the marketplace.

Later this token can be adjusted towards conflict resolution, between confronting parties,
without signifficantly affecting values of assets, towards which each of the confronting parties has delivered promises.

#``## Information-value markets 
`#metanet`.

<!-- #todo -->

## Formalisation

<!-- #todo Stricter notation and examples -->

$X$: Complete set of accessible variables, which can be used to construct conditions.

$T = τ_{0}, τ_{1}, ...$ : Set of non-overlapping and consecutive time periods, where $\sum τ_{i}$ is continous time function

$C^{τ_{i}} = \{c_{0}, c_{1}, c_{2}, ... \}$: Set of conditions, `active`, at time period $τ_{i}$

$(c_{i}, f) = (φ(λ(x)); f) \rightarrow (bool;f)$ where $x \in X$, $\lambda$ is any function, of $x$ and $φ$ is first order logic expression,
such that when its' value takes `truth`, we speak of the condition $c_{i}$ as the satisfied. $f$ is, the assosiated/promised action,
to be executed, whenever condition evaluates to true.

$ψ(F(C^{τ{i}})) =  ψ(2 ^ {C^{τ{i}}\rightarrow f}) = ψ(f_{0}, f_{1}, ..., f_{k}) \rightarrow  \alpha$
where $\alpha$ represents an action to be taken, $ψ$ is superfunction, that defines what happens, when there are multiple unctions,
assosiated with the condition set. $ψ$ = $\Sigma$, that is sum, unless stated otherwise. The motivation behind specyfying such is,
that functions

---

#### TODO

- [ ] Metanet $\leftrightarrow$ Information Value Markets
- [ ] Full featured example d
