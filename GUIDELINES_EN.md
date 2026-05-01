# Annotation Guidelines

---

## Overview

Welcome to the annotation task. In this task, you will be presented with a *tweet* along with its associated conversation thread, and you will be asked to classify it by indicating which class it belongs to given its context. This data will allow us to generate an open-access *dataset* that will be released to the scientific community, from which we will build a baseline model to enable comparisons and further development in this area at the national level.

## Concepts

We ask you to classify each *tweet* as **hate** or **not hate**. If classified as **hate**, you must indicate the target community the *tweet* is directed at, which can be **migrant communities**, **LGBTQ+ community**, **women**, or **indigenous peoples**. If it is a **not hate** tweet, you should still indicate the target community if any of the aforementioned groups are mentioned.

The concept of **hate** used in this work is tied to the definition of hate speech provided by the UN: *"Any kind of communication in speech, writing or behaviour, that attacks or uses pejorative or discriminatory language with reference to a person or a group on the basis of who they are, or in other words, based on their religion, ethnicity, nationality, race, colour, descent, gender or other identity factor."* For further reading on the topic, we recommend reviewing the [UN Plan of Action](https://www.un.org/en/genocideprevention/documents/advising-and-mobilizing/Action_plan_on_hate_speech_ES.pdf) for more definitions regarding hate speech.

In this task, we use the following narrowed definition of hate speech:

* **Hate Speech:** Text or message that constitutes an attack on or promotes discrimination against a person or group solely on the basis of their membership in one of the following groups: **migrant communities**, **LGBTQ+ community**, **women**, and **indigenous peoples**.

The main difficulty of this task lies primarily in two cases. The first is when hate speech does not use overtly pejorative language, but instead the complete phrase seeks to portray the mentioned group as less capable in any domain — physical, mental, financial, romantic, etc. — or less deserving of access to rights that ordinary members of the social context (i.e., those who do not belong to the mentioned group) enjoy with ease. The second case involves the use of pejorative language that, in context, is not considered discriminatory — for example, using such words when talking to a friend as a joke or in a sarcastic manner. This second case is of critical importance because, within the social and communicative context of Chilean dialect, this form of communication is highly frequent in informal situations or when interacting with peers.

For this task, we also introduce the concept of *context*, defined by the [RAE](https://www.rae.es/dpd/contexto) as *"The linguistic environment of a word, phrase, or fragment under consideration, on which its meaning often depends."* For this task, it is essential that when classifying the given *tweet*, you use the context to determine the true meaning of the phrase. In other words, there may be phrases that appear innocuous on their own, such as "yes, that's how it should be," but when reviewed in context, their meaning can change significantly. For example, the previous tweet could be a reply to the following tweet: "Only white people should control the country." While the reply does not use pejorative language against a specific group, in this case it seeks to diminish the rights of all those who do not belong to the group in question, and therefore, in context, the tweet does contribute to hate speech.

In general, these cases of hate rely on fallacious arguments, which in a sense helps facilitate their detection. Below are some common types, and the following links provide a deeper look at fallacies: [fallacy classifications](https://en.wikipedia.org/wiki/Fallacy#Classification), [types of fallacies](https://en.wikipedia.org/wiki/List_of_fallacies).

### Classes

For each *tweet*, first choose one of the following classes:

* **Hate** — If a *tweet*, in the context of its conversation thread, incites hatred according to the concept defined above. For example:
  * *"They call it marriage, good for those who fought for it, but for me it will always be a concept that unites a man and a woman. Simple."* — This tweet implies that same-sex marriage is not valid, suggesting that members of this community lack access to the same resources and rights as people who do not belong to this community.
  * *"I don't even know what to call them, because they're not a menstruating person or an ejaculating person — can we just call them f\*g and be done with it?"* — Uses pejorative language to refer to and mock an entire community, and this is not a case of joking among friends or self-irony.

* **Not Hate** — If a tweet does not contain hate. For example:
  * *"Annoying triple son-of-a-b\*tch (...) from: me / to: my anxiety"* — This tweet uses pejorative language, but it is directed at the author themselves to mock their own anxiety, so it does not constitute hate speech.

For each *tweet*, once classified into one of the above classes, determine if the tweet references any of the following communities:

* **LGBTQ+ Community** — For example:
  * *"I am heterosexual and I want my children to be heterosexual. Any problem?"* — **Hate**: arguing that parents define their children's sexual identity is incorrect and seeks to promote the idea that those with non-conventional sexual orientations are less valid.
  * *"Teacher, my mom told me you are gay."* — **Not Hate**: does not use pejorative language nor seek to discriminate; it seems to be a question directed at someone based on a comment made by the mentioned interlocutor.

* **Women** — For example:
  * *"There is life after being a feminazi. Some people evolve when they start reading and thinking. A round of applause."* — **Hate**: seeks to perpetuate the view of feminism as an ideological stance held by those of low intellectual level, thus falling into discrimination.
  * *"I'm so lonely, same as you, you fat b\*tch"* — **Not Hate**: although the sender is insulting someone, they make it clear that both are on equal footing regarding their loneliness (peer-level interaction).

* **Indigenous Peoples** — For example:
  * *"Idiots saying 'How exciting!!!' while most Chileans pay property taxes, unlike the Mapuche, who keep getting more benefits that the rest of us have to finance. Morons."* — **Hate**: uses fallacious arguments to support discrimination against indigenous peoples, claiming they do not pay taxes and live off state funds.

* **Migrant Communities** — For example:
  * *"All Venezuelans are lazy; they only come here to steal."* — **Hate**: uses fallacious arguments such as generalization to claim that the entire Venezuelan migrant community is lazy and criminal.
