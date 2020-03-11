*Everyone cries* is true
	iff 〚cries〛∈〚everyone〛
	iff {x: x cries} ∈ {A: {x: x is a person} ⊆ A}
	iff {x: x is a person} ∈ {x: x cries}

*Someone cries* is true
	iff 〚cries〛∈〚someone〛
	iff {x: x cries} ∈ {A: A ∩ {x: x is a person} ≠ ∅}
	iff {x: x cries} ∩ {x: x is a person} ≠ ∅

*Noone cries* is true
	iff 〚cries〛∈〚noone〛
	iff {x: x cries} ∈ {A: A ∩ {x: x is a person} = ∅}
	iff {x: x cries} ∩ {x: x is a person} = ∅

*Noone* is true iff {A: |A ∩ {x: x is a person}| = 0}
*Someone* is true iff {A: |A ∩ {x: x is a person}| > 0}
*Everyone* is true iff {A:  |{x: x is a person} ⊆ A| = |{x: x is a person|}}<big><strong>???</strong></big>

### Quantifiers

#### Generalized Quantifiers

> 〚every student〛 = {A: 〚student〛 ⊆ A}
> 〚some student〛 = {A: 〚student〛 ∩ A} ≠ ∅
> 〚no student〛 = {A: 〚student〛 ∩ A} = ∅
> 〚two student〛 = |{A: 〚student〛 ∩ A}| = 2
> 〚most student〛 = |{A: 〚student〛 ∩ A}| > |{ A: 〚student〛 ∩ A’ }|

#### Quantificational Determiners

```
[Every 		girl] 		laughs
 Determiner	Restrictor	Scope
```

**Restrictor** denotes a set of individuals, just like the **scope**.

**Determiner** denotes a relation between **sets**.

```
[Every					student]			learns
 relation between sets	set of individuals	set of individuals
```

So, the specific relations denoted by specific determiners are as follows:

*every* 	=>	〚every P〛 = { A: 〚P〛 ⊆ A }
*some*	=>	〚some P〛 = { A: 〚P〛 ∩ A ≠ ∅}
〚every〛 = ⊆
〚some〛 = overlaps
*and so on…*

##### Logical Properties of Quantifying Determiners

Quantifiers can be grouped in **different semantic natural classes** and mathematical properties of determiners play a key role in understanding **empirical phenomena** involving natural language quantification.

Let *A*, *B*, and *C* be sets of individuals, A relation *R* between sets is

|                |      |                                                              |
| -------------- | ---- | ------------------------------------------------------------ |
| *Reflexive*    | iff  | for every *A*; *R* holds of *A* and *A*                      |
| *Transitive*   | iff  | for every *A*, *B*, and *C*; if *R* holds of *A* and *B* and *R* holds of *B* and *C*, then *R* holds of *A* and *C* |
| *Symmetric*    | iff  | for every *A* and *B*; if *R* holds of *A* and *B*, then it holds of *B* and *A* |
| *Conservative* | iff  | for every *A* and *B*; *R* holds of *A* and *B* if and only if it holds of *A* and *A* ∩ *B* |
| *Left UE*      | iff  | for every *A*, *B*, and *C* such that *A* ⊆ *C*; if *R* holds of *A* and *B*, then *R* holds of *C* and *B* |
| *Right UE*     | iff  | for every *A*, *B*, and *C* such that *B* ⊆ *C*; if *R* holds of *A* and *B*, then *R* holds of *A* and *C* |
| *Left DE*      | iff  | for every *A*, *B*, and *C* such that *C* ⊆ *A*, if *R* holds of *A* and *B*, then *R* holds of *C* and *B* |
| *Right DE*     | iff  | for every *A*, *B*, and *C* such that *C* ⊆ *B*, if *R* holds of *A* and *B*, then *R* holds of *A* and *C* |

##### Generalization of Determiners as Conservative

A relation *R* is conservative iff for every *A* and *B*; *R* holds of *A* and *B* iff *R* holds of *A* and *A* ∩ *B*.

> *Every student smokes* is true iff *Every student is a student and smokes*
> 		A				 B								A						A		∩		B

**Proof**

```
1 Show if 〚every〛 holds of A and B iff 〚every〛 holds of A and A∩B, then 〚every〛 is conservative
2 | Show 〚every〛 holds of A and B iff 〚every〛 holds of A and A∩B
3 | | Show if 〚every〛 holds of A and B, then 〚every〛 holds of A and A∩B
4 | | | 〚every〛 holds of A and B											assumption
5 | | | A ⊆ B															meaning of every
6 | | | A ∩ B = A															set theory
7 | | | A ⊆ A																set theory
8 | | | A ⊆ A ∩ B															from 6,7
9 | | | 〚every〛 holds of A and A ∩ B
10| | Show if 〚every〛 holds of A and A∩B, then 〚every〛 holds of A and B
11| | | 〚every〛 holds of A and A∩B											assumption
12| | | A ⊆ A ∩ B														meaning of every
13| | | A ∩ B = A															12, set theory
14| | | A ⊆ B																set theory
15| | | 〚every〛 holds of of A and B
```

**Determiners** in all lnaguages are always **conservative**!

Inverting a noconservative quantifier **allnon**.

〚*allnon A are B*〛 is true iff *A’* ⊆ *B*
Allnon students smoke != Allnon students are students who smoke.

Allnon students are not even students! Therefore it’s not a quantifier.

Is *only* conservative?

Only students smoke != Only students are students who smoke.

This is not true. There are non-smoker students. So *only* is not a determiner. It’s some kind of an adverb, as it can appear in more places than usual determiners:

Mary only eats pizza
Only John slept
Only some students were there
I bought only 3 books

#### NPI licensing

NPIs are items that are licensed only the local scope of a "negative” expressions such as *any*, *ever*, *budge an inch*, *lift a finger*…

*John has <u>ever</u> been to Moscow.
John hasn’t <u>ever</u> been to Moscow.

NPIs are grammatical **in the scope of** *no*, *at most*,, but **not in the scope of** *every*, *some*, *at least*.

*Every student has ever been o Moscow
No student has ever been to Mostow.
*Some student has ever been to Mostow.

NPIs are grammatical **in the restrictor of** *every*, *no*, *at most*, **but not in the restrictor of** *some*, *at least*…

Every student who has ever been to Moscow liked it.
No student who has ever been to Moscow liked it.
*Some student who has ever been to Moscow liked it.

These are all linked to entailments of the determiners –whether upward or downward, or in the scope or in the restrictor.– The logical property of **negation** is the **Downward Entailment (right or left)**.

*No student called* entails *no blond student called*. (restrictor)
*No student eats vegetables* entails *no student eats kale*. (scope)
So *no* is downward entailing in both in its restrictor and scope. Therefore, it licences NPIs in both too.
*No student who has ever been to Moscow called* and *No student has ever eaten vegetables*

*Some students called* does not entail *some blond students called*.
*Some students eat vegetables* does not entail *some students eat kale*.
So *some* is not downward entailing at all. Therefore, it doesn’t licence NPIs anywhere.
**Some students who has ever been to Moscow called* and * *Some students has ever eaten kale*

*Every student called* entails *every blond student called*.
*Every student eats vegetables* does not entail *every student eats kale*.
So *every* is DE in its restrictor, but not in its scope. Therefore, it only licences NPIs in its restrictor.
*Every student who has ever been to Moscow called* and **Every student has ever eaten vegetables*

#### Definite Determiner, Presuppositions, and Compositionality

**Assertion** and **Presupposition** are two components a speaker conveys when uttering a sentence:

*Mary quit smoking*
**Assertion**: Mary isn’t a smoker right now.
**Presupposition**: Mary used to be a smoker.

Testing the presupposition:
**Negating the sentence**: *Mary hasn’t quit smoking* still presupposes that she was a smoker.
**Question forming**: *Did Mary quit smoking?* still presupposes that she was a smoker.

##### The Definite Determiner

There will be **a midterm** on March 30th. (No presupposition)
**The midterm** will be on March 30th. (There is a specific midterm)
**The midterm** will not be on March 30th. (Still, there is a midterm)
**The sixth midterm** will be on March 30th. (There is no 6th midterm, therefore the sentence is **infelicitous**)
**The final** will be on January 14th. (The final exists, but it will not be on 14th of January, therefore the sentence is **false**)

**The Fregean View**: like a proper name, a definite description refers to an individual. What individual? We find the individual by looking for things that are in the set denoted by the description/restrictor. Also, we know that there mmust be a unique such individual.
〚the A〛 = the unique x s.t. x ∈ 〚A〛

Same tests apply to definite determiners, but also **Hey, wait a minute!** test:

A: The French teacher of LING 305 is late.
B: Hey, wait a minute! The teacher of 305 is not French!
B: *Hey, wait a minute! She is not sick!

##### Context Dependency of Definite Determiner

*No dogs are aggressive today* doesn’t convey the meaning of *There are no dogs in the entire world that are aggressive today* but *No dogs in this shelter/on campus/on my street etc.* is aggressive today.

So, the intended denotation is: 〚dog〛∩ C (context)

So, 〚the A〛 presupposes that |〚A〛∩ C |= 1

#### Sense and Reference

Sense can refer to different entities in different worlds

> *The dog which lives in Paula’s house* can refer to Shelby or Hannibal

Reference’s meaning doesn’t change based on state.

> *The dog* can only refer to one specific dog

Proper names are same in every world, they only have referents. (Rigid Designators)

Definites can pick different referents in different worlds, because they have a sense.

**Informative / Can be wrong** *The president of US is Trump*
**Tautology** *Trump is Trump*

