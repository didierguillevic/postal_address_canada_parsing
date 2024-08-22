# postal_address_canada_parsing
Fine-tuning a base model for a token classification task (postal address parsing)

**Steps**
- Step 0: get millions of postal addresses from [openaddresses.io](https://batch.openaddresses.io/data#map=0/0/0)
- Step 1: select columns of interests and create train / validation / split
- Step 2: attempt to "de-normalize" the postal addressess so that they are more likely to represent what we get in real life.
- Step 3: fine-tune a fill-mask base model for a token classification; e.g. base_model = [google-bert/bert-base-multilingual-uncased](https://huggingface.co/google-bert/bert-base-multilingual-uncased)
- Step 4: demo time on HuggingFace Spaces: [Didier/Postal_address_canada_parsing](https://huggingface.co/spaces/Didier/Postal_address_canada_parsing)
