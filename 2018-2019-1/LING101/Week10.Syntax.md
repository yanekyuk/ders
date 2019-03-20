### CHAPTER 3

# Syntax: The Sentence Patterns of Language

## Hmm, interesting...

- Sentences are composed of discrete units that are combined by rules, thus explaining how speakers can store infinite knowledge in a finite space.

- The **rules of syntax** combine words into phrases and phrases into sentences.

- The rules of the syntax also specify the **grammatical relations** of a sentence, such as **subject** and **direct object**.

- The following hierarchical diagrams, also called **tree diagrams**, illustrate the same point:

  ```mermaid
  graph TD;
  	mg1["Main Group"];mg2["Main Group"]
  	sg1["Sub Group"];sg2["Sub Group"]
  	old1["Old"];old2["Old"]
  	men1["men"];men2["men"]
  	and1["and"];and2["and"]
  	wom1["women"];wom2["women"]
  	mg1-->sg1; 
  	mg1-->and1; mg1-->wom1;	mg2-->old2; mg2-->sg2;
  	sg1-->old1; sg1-->men1;
  	sg2-->men2; sg2-->and2; sg2-->wom2;
  ```

- `For sale: an antique desk suitable for lady with thick legs and large drawers.`In this example ambiguity is a result of different structures, thus it is an instance of **structural ambiguity**.

- Sentence structure glossary:

| abbr. | expl.                     |
| ----- | :------------------------ |
| Det   | determiner _(a, an, the)_ |
| N     | noun                      |
| V     | verb                      |

- _The child found a puppy._ =>

  ```mermaid
  graph TD;
  	np1["noun phrase"];vp1["verb phrase"];np2["noun phrase"]
  	root---np1; np1---the; np1---child;
  	root---vp1; vp1---found; vp1---np2;
  	np2---a; np2---puppy;
  	
  
  ```

- The natural groupings or parts of a sentence are called **constituents**. 

  - **Test I**: If a group of words can stand alone, for example, as an answer to a question, they form a constituent.
  - **Test II**: If a group of words can be replaced by a pronoun or a word like _do_, it forms a constituent.
  - **Test III**: If a group of words can be moved, they form a constituent.

- As before, our knowledge of the **constituent structure** of a sentence may be graphically represented by a tree diagram. The tree diagram for the sentence "The puppy played in the garden" is as follows:

  ```mermaid
  graph TD;
  	c1["const."];c2["const."];c3["const."];c4["const."];
  	root---c1; c1---the; c1---puppy; root---c2; c2---played; 
  	c2---c3; c3---in; c3---c4;
  	c4---the2["the"]; c4---garden;
  ```

- Experimental evidence has shown that speakers do not mentally represent sentences as strings of words but rather in terms of constituents.

- A family of expressions that can substitute for one another without loss of grammaticality is called a **syntactic category**.

- _The child_, _a police officer_, _John_, and so on belong to the syntactic category **noun phrase (NP)**, one of several categories in English and all languages.

- The expression _found a puppy_ is a **verb phrase (VP)**. A verb phrase always contains a **verb (V)**, and it may contain other categories, such as a noun phrase or **prepositional phrase (PP)**, which is a preposition followed by an NP, such as _in the park_, _on the roof_, _with a balloon_.

- Lexical and functional categories are:

| Phrasal categories                                           | Lexical categories                                           |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Noun Phrase (NP) \| _men, the man, the man with a telescope_ | Noun (N) \| _puppy, boy, man, soup, happiness, fork, kiss, p_ |
| Verb Phrase (VP) \| _sees, always sees, rarely sees the man, often sees the man with a telescope_ | Verb (V) \| _find, run, sleep, throw, realize, see, try, want, believe_ |
| Adjective Phrase (AP) \| _happy, very happy, very happy about winning_ | Adjective (A) \| _red, big, happy, candid, hopeless, fair, idiotic, lucky_ |
| Prepositional Phrase (PP) \| _over, nearly over, nearly over the hill_ | Preposition (P) \| _up, down, across, into, from, by, with, over_ |
| Adverbial Phrase (AdvP) \| _brightly, more brightly, more brightly than the sun_ | Adverb (Adv) \| _again, always, brightly, often, never, very, fairly_ |

- The category **determiner (Det)**, which includes the articles _the_ and _a_, as well. **Demonstratives** such as _this_, _that_, _these_, and _those_. **Quantifiers**, such as _each_ and _every_. Another less familiar category is **tense (T)**, which includes the **modal** auxilliaries _may, might, can, could, must, shall, should, will,_ and _would_, and abstract tense morphemes. **T** and **Det** are **functional categories**, so called because their members have grammatical functions rather than descriptive meanings.

- The modals belong to a larger class of verbal elements traditionally referred to as **auxiliaries** or **helping verbs**, which also include_have_ and _be_ in sentences such as _John is dancing_ or _John has danced_.

- A **complement** is defined as a phrasal category that may occur next to a head, and only there, and which elaborates on the meaning of the **head**.

- In addition, a phrase may have an element preceding the head. These elements are called **specifiers**.

  - I head [Pavarotti sing an aria].
  - Betty made [Jane wary of snakes].

  ```mermaid
  graph TB;
  	NP--specifier---the;NP---NP2["NP"];
  	NP2---mother; NP2---jam["of James Whistler"];
  	VP--specifier---Pavorotti; VP---VP2["VP"];
  	VP2---sing; VP2---ar["an aria"];
  	AP--specifier---Jane; AP---AP2["AP"];
  	AP2---wary; AP2---snk["of snakes"];
  	PP--specifier---just; PP---PP2["PP"];
  	PP2---over; PP2---hil["the hill"];
  ```

  - In each of the phrases the head and its complement are under the same **node**, reflecting the fact that the complement has an important relationship with the meaning of the head. We refer to categories under the same node as **sisters**.

  ```mermaid
  graph TD;
  	XP---spe["specifier of X"];
  	XP---X-Bar; X-Bar---x1["X (head)"]; X-Bar---comX["complement of X"]
  ```

  ```mermaid
  graph TD;
  	NP---N';N'---N;N---oxygen;
  	VP---V';V'---V;V---sleeps;
  	AP---A';A'---A;A---beautiful;
  	PP---P';P'---P;P---in;
  ```

  ```mermaid
  graph TD;
  	S---NP;S---VP;
  	NP---det;det---the;NP--N'---N;N---child;
  	VP---V';V'---V;V---found;V'---NP2["NP"];NP2--det---a;NP2--N'---N2["N"];N2---puppy;
  ```

- A tree diagram with syntactic category information is called a **phrase structure tree (PS tree)** or a **constituent structure tree**.

- Every higher node is said to **dominate** all the categories that can be traced down the tree beneath it. A node is said to **immediately dominate** the categories one level below it. The **subject** of a sentence is the NP immediately dominated by S and the **direct object** is the NP immediately dominated by V'.

- _Find_ is a **transitive verb** and it requires an NP complement (direct object). _Sleep_ is an **intransitive verb**; it cannot take an NP complement.

- An example of **declarative sentence** is *The boy will dance*, and of **yes-no question** is *Will the boy dance?*The yes-no question is formed via **Move (transformational rule)**: *The boy must sleep* becomes *Must the boy sleep?*

- When transformations apply **deep** and **surface structure** of sentence differ:

  - **active-passive**
    - The cat chased the mouse. -> The mouse was chased by the cat.
  - **there-sentences**
    - There is a bear in your closet. -> A bear is in your closet.
  - **PP preposing**
    - Tom Dooley stabbed her with his knife. -> With his knife Tom Dooley stabbed her.

- The transformation Move acts on phrase structures without regard to the particular words that the structures contain, that is, it is **structure dependent**.

- The point of variations in between languages are called **parameters**.

## Summary

- Speakers of a language recognize ambiguities, know when different sentences mean the same thing, such as **subject** and **direct object**. This kind of knowledge form their knowledge of the **rules of syntax**.
- Sentences have structure that can be represented by **phrase structure trees** containing **syntactic categories**. PS trees reflect the speaker's mental representation of sentences. Ambiguous sentences may have more than one phrase structure tree.
- There are different kinds of syntactic categories: **Phrasal categories**, such as NP and VP, are composed of other syntactic categories; **lexical categories**, such as Noun and Verb, and **functional categories**, such as Det and T, often correspond to individual words. The hierarchical structure of the phrasal categories is universal and is specified by the **X-Bar schema**, consisting of a **specifier**, a **head**, and its **complements** and **adjuncts**.
- **Phrase structure rules** can express the particular order of elements within the phrase for each language.
- The **lexicon** represents the knowledge that a speaker has about the vocabulary of their language. This knowledge includes the syntactic categories of words as well as the **sub-categorization** or **c-selection** properties of particular lexical items that specify the complements they can take, for example whether a verb is **transitive** or **intransitive**.  The lexicon also contains semantic information, including the **s-selection** . Selectional restrictions must be satisfied in the **d-structure** representation of the sentence.
- **Transformational rules** such as Move and *do-insertion* account for relationships between sentences such as declarative and interrogative pairs, including *wh* questions. Transformations such as Move can relocate constituents. The output of the transformational rules is the **s-structure** of a sentence, the structure that most closely determines how the sentence is to be pronounced (or signed).
- The basic design of language is universal. Universal Grammar specifies that syntactic rules are **structure-dependent** and that movement rules may not move phrases out of certain structures such as certain types of clauses, among many other constraints, including a need to not violate the X-bar schema.