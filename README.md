# Noisy Sentences Dataset

[![DOI](https://zenodo.org/badge/596943135.svg)](https://zenodo.org/badge/latestdoi/596943135)

550K sentences in 5 European languages augmented with noise for training and evaluating spell correction tools or machine learning models. We have constructed our dataset to cover representatives from the language families used across Europe.
- Germanic - English, German;
- Romance - French;
- Slavic - Bulgarian;
- Turkic - Turkish;

**Use case example:** Apply language models or other techniques to compare the sentence pairs and reconstruct the original sentences from the augmented ones. You can use a single multilingual solution to solve the challenge or employ multiple models/techniques for the separate languages. Per-word dictionary lookup is also an option.

## Files

*   **train.csv** - the training set
*   **test.csv** - the test set

Because of an ongoing [Kaggle competition](https://www.kaggle.com/competitions/ml-olympiad-multilingual-spell-correction/), the testing set labels will be released in March 2023.

## Columns

*   `Id` - unique id for each sentence pair
*   `Language` - one of `en` (English), `bg` (Bulgarian), `tr` (Turkish), `fr` (French), `de` (German)
*   `Text` - noisy text
*   `Expected` - original sentence before augmentation

## Cite

```bibtex
@software{Cholakov_Noisy_Sentences_Dataset_2023,
  author = {Cholakov, Radostin},
  doi = {10.5281/zenodo.7602333},
  month = {2},
  title = {{Noisy Sentences Dataset}},
  url = {https://github.com/radi-cho/noisy-sentences-dataset},
  version = {0.0.1},
  year = {2023}
}
```

## Credits
The sentences in our dataset are sourced from [Wikipedia](https://en.wikipedia.org/wiki/Main_Page). The contents of Wikipedia are licensed under the [Creative Commons 3.0 License](https://en.wikipedia.org/wiki/Wikipedia:Text_of_the_Creative_Commons_Attribution-ShareAlike_3.0_Unported_License).
