# Link to our mirror: https://api.bbvr.ai/public/two-million-bluesky-posts/


## 2 Million Bluesky Posts

This dataset contains 2 million public posts collected from Bluesky Social's firehose API, intended for machine learning research and experimentation with social media data.

The with-language-predictions config contains the same data as the default config but with language predictions added using the glotlid model.
Dataset Details
Dataset Description

This dataset consists of 2 million public posts from Bluesky Social, collected through the platform's firehose API. Each post contains text content, metadata, and information about media attachments and reply relationships.

- **Curated by**: Alpin Dale
- **Language(s) (NLP)**: Multiple (primarily English)
- **License**: Dataset usage is subject to Bluesky's Terms of Service


## Uses

This dataset could be used for:

- Training and testing language models on social media content
- Analyzing social media posting patterns
- Studying conversation structures and reply networks
- Research on social media content moderation
- Natural language processing tasks using social media datas

## Dataset Structure

The dataset is available in two configurations:
### Default Configuration

Contains the following fields for each post:

- **text**: The main content of the post
- **created_at**: Timestamp of post creation
- **author**: The Bluesky handle of the post author
- **uri**: Unique identifier for the post
- **has_images**: Boolean indicating if the post contains images
- **reply_to**: URI of the parent post if this is a reply (null otherwise)

### With Language Predictions Configuration

Contains all fields from the default configuration plus:

- **predicted_language**: The predicted language code (e.g., eng_Latn, deu_Latn)
- **language_confidence**: Confidence score for the language prediction (0-1)

Language predictions were added using the [glotlid](https://huggingface.co/cis-lmu/glotlid) model via fasttext.

## Bias, Risks, and Limitations
The goal of this dataset is for you to have fun :)
