# Refactoring Requirements with RQT

Hi! Welcome to the guide on improving your requirement's quality. By using the **Requirements Quality Toolkit**, you can automatically analyze your requirements for potentially ambiguities. Eliminating those ambiguities can be a process of eliciting more information from the customer/client. Below are some realistic examples of refactoring requirements using RQT.


## Eliminating Undefined Terms


![Undefined Terms Report output](https://user-images.githubusercontent.com/53841072/87467806-22792e00-c5de-11ea-9947-3ddc9186c4bb.png)

If there are undefined terms, add definitions for those terms in a data dictionary, glossary, or text file. 

In this example above, we have three undefined term warnings - **User Interactions subsystem**, **authorized user**, and **managed data ingest task** highlighted in gray. Adding a definition for each of these undefined terms fixes the undefined term warnings.

![enter image description here](https://user-images.githubusercontent.com/53841072/87477739-3af14480-c5ee-11ea-8e76-45372bef04a7.png)


## Eliminating Superfluous Infinitives


![enter image description here](https://user-images.githubusercontent.com/53841072/87487167-8e6d8d80-c602-11ea-9c5a-4b4b1cca3971.png)

To sneeze, to smash, to cry, to shriek, to jump, to dunk, to read, to eat, to slurp—all of these are infinitives. An infinitive will almost always begin with to followed by the simple form of the verb.

**To + Verb = Infinitive**

If the intent of using "be able to" or "be capable of" type wording is to communicate the system will only need to do the required action based on some condition, trigger, or state, then it is best to state the condition, trigger, or state as part of the requirements.

In this example above, we have an infinitive **to configure** highlighted in yellow. The phrase **allow an authorized user to configure** is unnecessarily verbose. Removing the infinitive and creating a separate requirement restricting unauthorized users would fix the infinitive warning.



![enter image description here](https://user-images.githubusercontent.com/53841072/87489899-d7751000-c609-11ea-86ca-e67283a64cec.png)

## Eliminating Pronouns

Repeat nouns in full instead of using pronouns to refer to nouns in other need or requirement statements. Pronouns can also indicate multiple "thoughts" in a requirement. Separate out thoughts into multiple requirements or add definitions.

In this example above, the pronoun **it** indicates that a definition can be extracted from the requirement. Adding a definition can eliminate the pronoun and fix the pronoun warning.

![enter image description here](https://user-images.githubusercontent.com/53841072/87614890-f392b300-c6d6-11ea-821a-68a462a27171.png)

## Eliminate Temporal Dependencies

Define temporal dependencies explicitly instead of using indefinite temporal keywords. Indefinite temporal keywords such as "eventually", "until", "before", "when", "after" can cause confusion or unintended meaning. These words should be replaced by specific timing constraints or specific causal actions.

In this example above, the temporal dependency **before** signals a non-specific timing. Creating a separate requirement with a specific causal action can eliminate the temporal dependency and fix the warning.

![enter image description here](https://user-images.githubusercontent.com/53841072/87624758-1d0b0900-c6ee-11ea-934f-53f2496a6588.png)

## Eliminating Indefinite Articles

Use definite article "the" or no article rather than the definite article "a". When referring to entities, use of the indefinite article can lead to ambiguity.

In this example above, the indefinite articles **a** can create confusion in verification and validation. Removing the indefinite article, and using the definite article or no article can eliminate the indefinite article and fix the warning.

![enter image description here](https://user-images.githubusercontent.com/53841072/87703715-e7533800-c760-11ea-93b7-a9647314e6d2.png)

## Eliminating Combinators

![enter image description here](https://user-images.githubusercontent.com/53841072/87708402-4799a800-c768-11ea-82fc-916377eb764a.png)


Combinators are words that join clauses, such as "and", "or", "then", "unless", "but", "as well as", "however", etc. Their presence in a requirement usually indicates that *multiple requirements* should be written.

In this example above, the first combinator **and** indicates that this requirement is actually multiple requirements. The second **and** is part of a term and is not considered a combinator. Splitting the compound requirement into multiple singular requirements eliminates the first combinator and fixes the warning.

![enter image description here](https://user-images.githubusercontent.com/53841072/87709047-487f0980-c769-11ea-8b9e-32cb50609909.png)

## Eliminating Not

![enter image description here](https://user-images.githubusercontent.com/53841072/87730957-dc170100-c78e-11ea-9a8d-2dfcc85290a9.png)

The presence of "not" in a need or requirement statement implies "not ever", which is impossible to verify in a finite time. Rewriting the need or requirement statement to avoid the use oof 'not" results in a need or requirement statement that is clearer and is verifiable or able to be validated.

In this example above, the presence of **not** makes the requirement hard to verify. Rewriting the requirement avoiding the use of not fixes the warning making the requirement easier to verify.

![enter image description here](https://user-images.githubusercontent.com/53841072/87734314-ea1d4f80-c797-11ea-855b-98cb198a9879.png)


