# CAPP Dataset: Context Aware Polite Paraphrase Dataset

[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

## Description

This repository contains information about the ***Context Aware Polite Paraphrase (CAPP) dataset*** - a dialogue-style corpus of rude utterances and corresponding polite paraphrases, with samples accompanied by additional context in the form of prior turns from the dialogue. The original paper [**Demonstrations Are All You Need: Advancing Offensive Content Paraphrasing using In-Context Learning**][Arxiv Paper] was accepted in [ACL 2024 Findings][ACL 2024]. We also provide the generated paraphrases for the different methods described in the paper. 

## [Data](https://github.com/anirudhsom/CAPP-Dataset/tree/main/Dataset)

- Within the CAPP dataset, the [training split](https://github.com/anirudhsom/CAPP-Dataset/blob/main/Dataset/train.csv) has 7939 samples and the [test split](https://github.com/anirudhsom/CAPP-Dataset/blob/main/Dataset/test.csv) has 1120 samples. Each sample will always have a rude utterance and a polite paraphrase. Furthermore, about 55% of the training data and 53% of the test data also has prior dialogue turn utterances to provide additional context.

- The following notebook will help you load and inspect the training and test data splits: [notebook](https://github.com/anirudhsom/CAPP-Dataset/blob/main/Dataset/notebook.ipynb)

- Dialogues for samples with multiple dialogue turns will be separated using the [SEP] separator. For example:
  ```
  How long have we been here? [SEP] It's been 2 days and 7 hours. [SEP] What will happen to us?
  ```

## [Generated Paraphrases](https://github.com/anirudhsom/CAPP-Dataset/tree/main/Generated_Paraphrases)

Here, we describe the underlying file structure to query the generated paraphrases for the following models:

1. text-davinci-003
2. gpt-3.5-turbo-instruct
3. gpt-3.5-turbo-0613
4. gpt-3.5-turbo-1106
5. Vicuna-13b

***

## Citation

```
@article{som2023demonstrations,
  title={Demonstrations Are All You Need: Advancing Offensive Content Paraphrasing using In-Context Learning},
  author={Som, Anirudh and Sikka, Karan and Gent, Helen and Divakaran, Ajay and Kathol, Andreas and Vergyri, Dimitra},
  journal={arXiv preprint arXiv:2310.10707},
  year={2023}
}
```

## Contact

Please report any issues to [Github Issues][Git Issues].

For any questions, please contact: Anirudh Som (anirudh.som@sri.com)


## Acknowledgement

This material is based upon work supported by the Defense Advanced Research Projects Agency (DARPA) under Contract No. HR001122C0032. Any opinions, findings and conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views or policies of DARPA, the Department of Defense or the U.S. Government.

## License

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[ACL 2024]: https://2024.aclweb.org/
[Arxiv Paper]: https://arxiv.org/abs/2310.10707
[Git Issues]: https://github.com/anirudhsom/CAPP-Dataset/issues

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
