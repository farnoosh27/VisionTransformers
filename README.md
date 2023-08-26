# What are transformers in the field of NLP?
Transformers are an innovative kind of deep learning architecture used in Natural Language Processing. They stand out in handling sequences, like sentences, by employing self-attention mechanisms to grasp word relationships. This enables them to comprehend context without being limited by word order. Transformers consist of elements like multi-head attention, positional encoding, and feedforward networks. They're applied in models such as BERT for contextual word understanding, GPT for text creation, and T5 for diverse tasks. Transformers have transformed NLP and surpassed previous models by better grasping language context.

# What is Embedding?

Before delving into the details of transformer architecture, it may be a good idea to establish a foundation on the **Embedding**. I found this video by Jay Allamar about [Word2vec algorithm](https://www.youtube.com/watch?v=ISPId9Lhc1g), and reading this [article](https://jalammar.github.io/illustrated-word2vec/)

Transformers introduce a cutting-edge architecture comprising two main elements: the **encoder** and the **decoder**.

## Encoder

The encoder handles input sequences, such as sentences. It resembles the comprehension component. It evaluates the importance of each word relative to the others. This process occurs in parallel multiple times, considering word positions. Following this, it enhances the understanding of each individual word.

## Decoder

The decoder generates output sequences, like translations, based on the encoder's comprehension. It takes into account its own words and the input sequence. With attention to word importance and positions, it constructs the final output.

For tasks like translation, these components collaborate. During the learning process, the model adjusts its parameters to align its output with the desired result.

To sum up, transformers excel at capturing word relationships and context, making them invaluable for various language tasks. They harness attention, parallel processing, and refinement steps to truly excel in this domain.
