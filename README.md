# NLP-Project
#### English to Arabic translation using fine tuned pretrained transformer
by:
- Mohamed Tarek 
- Fady Hany
- Mostafa Sudany

### Dataset: OPUS-100
OPUS-100 is an English-centric multilingual corpus covering 100 languages. It was randomly sampled from the OPUS collection.
OPUS-100 was used for the experiments in the paper "Improving Massively Multilingual Neural Machine Translation and Zero-Shot Translation". Please cite that paper if you use this corpus and, pleae, also acknowledge OPUS.
	The OPUS collection is comprised of multiple corpora, ranging from movie subtitles to GNOME documentation to the Bible. We did not curate the data or attempt to balance the representation of different domains, instead opting for the simplest approach of downloading all corpora for each language pair and concatenating them.
	The dataset is split into training, development, and test portions. We randomly sampled up to 1M sentence pairs per language pair for training and up to 2000 each for development and test. To ensure that there was no overlap (at the monolingual sentence level) between the training and development/test data, we applied a filter during sampling to exclude sentences that had already been sampled. Note that this was done cross-lingually so that, for instance, an English sentence in the Portuguese-English portion of the training data could not occur in the Hindi-English test set.
	OPUS-100 contains approximately 55M sentence pairs. Of the 99 language pairs, 44 have 1M sentence pairs of training data, 73 have at least 100k, and 95 have at least 10k.
### Model Parameters 
The model is a fine tuned version of the Helsinki-NLP/opus-mt-en-ar which is a transformer trained on the OPUS-100 dataset and evaluated with the BLEU benchmark 

## License 
this code is licensed under the Apache-2.0 license, this may not apply to the dataset or the pretrained model
