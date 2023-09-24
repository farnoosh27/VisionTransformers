## History

| Paper                                                     | Method            | Domain                        | Year       |
|-----------------------------------------------------------|-------------------|-------------------------------|------------|
| [Attention is all you need](https://arxiv.org/abs/1706.03762)                               | Transformer       | Natural Language Processing  | 2017       |
| An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale | Vision Transformer | Computer Vision               | 2020/2021  |

## Application of transformers in computer vision

## What are transformers in the field of NLP?

Transformers are an innovative kind of deep learning architecture used in Natural Language Processing. They stand out in handling sequences, like sentences, by employing self-attention mechanisms to grasp word relationships. This enables them to comprehend context without being limited by word order. Transformers consist of elements like multi-head attention, positional encoding, and feedforward networks. They're applied in models such as BERT for contextual word understanding, GPT for text creation, and T5 for diverse tasks. Transformers have transformed NLP and surpassed previous models by better grasping language context.

## What is Embedding?

Before delving into the details of transformer architecture, it may be a good idea to establish a foundation on the **Embedding**. I found this video by Jay Allamar about [Word2vec algorithm](https://www.youtube.com/watch?v=ISPId9Lhc1g), and reading this [article](https://jalammar.github.io/illustrated-word2vec/).

Transformers introduce a cutting-edge architecture comprising two main elements: the **encoder** and the **decoder**.

## Encoder
The encoder handles input sequences, such as sentences. It resembles the comprehension component. It evaluates the importance of each word relative to the others. This process occurs in parallel multiple times, considering word positions. Following this it enhances the understanding of each individual word.

## Decoder
The decoder generates output sequences, like translations, based on the encoder's comprehension. It takes into account its own words and the input sequence. With attention to word importance and positions, it constructs the final output.

For tasks like translation, these components collaborate. During the learning process, the model adjusts its parameters to align its output with the desired result.

To sum up, transformers excel at capturing word relationships and context, making them invaluable for various language tasks. They harness attention, parallel processing, and refinement steps to excel in this domain truly.

## Transformer Architecture Components

### Encoder

The **encoder** handles the input sequence, breaking it down into meaningful representations through a series of layers:

- **Self-Attention Mechanism:** This core component allows the model to weigh the importance of each word relative to all others, capturing relationships and context regardless of position.

- **Multi-Head Attention:** The encoder employs multiple parallel self-attention mechanisms, or "heads," capturing diverse relationships and nuances.

- **Positional Encoding:** To account for word order, positional encoding is added to input embeddings, conveying word position information.

- **Feedforward Neural Network:** After attention stages, a feedforward neural network refines word representations using captured context.
### Decoder

The **decoder** generates the output sequence based on the processed input sequence:

- **Self-Attention Mechanism (Decoder-side):** This mechanism enables the decoder to focus on its own generated output, avoiding undue attention to irrelevant input parts.

- **Multi-Head Attention (Encoder-Decoder Attention):** The decoder aligns its output with relevant parts of the input by attending to the encoder's output, which is crucial for tasks like translation.

- **Positional Encoding:** Similar to the encoder, the decoder employs positional encoding to understand word order in generated sequences.

- **Feedforward Neural Network:** The decoder's feedforward network refines generated output using both input sequence and preceding words.

The transformer architecture excels at capturing context and dependencies in sequences, making it highly effective for various NLP tasks. The self-attention mechanisms, multi-head attention, and feedforward networks collectively empower transformers to understand relationships, context, and nuances in data.
