# Annotations for the Novel Visual Concept dataset

Created by [Junhua Mao](http://www.stat.ucla.edu/~junhua.mao/)

## Citation
If you find this dataset and annotations useful in your research, please consider citing:

    @article{mao2015learning,
      title={Learning like a Child: Fast Novel Visual Concept Learning from Sentence Descriptions of Images},
      author={Mao, Junhua and Xu, Wei and Yang, Yi and Wang, Jiang and Huang, Zhiheng and Yuille, Alan},
      journal={ICCV},
      year={2015}
    }

## Format

This dataset contains two JSON files: one for training and validation set, one for testing set.
The JSON file is organized as follows:

The root is a key-value dictionary:
- 'version': version of the dataset
- 'concepts': a list of the novel visual concepts
- 'images': a list, each element of the list is a dictionary:
  - 'concept': novel concepts for the image
  - 'image_id': unique id for the image
  - 'image_name': file name for the image
  - 'train_val_test_split': 'train' or 'val' or 'test'
  - 'sentences': a list, each element of the list is a dictionary:
    - 'raw': a string which is the raw annotated sentence
    - 'tokens': tokenized sentence, NOT includes the period at the end
    - 'sentence_id': unique id for the sentence
    - 'image_id': unique image id that the sentence belongs
    
## License

The annotations in this dataset belong to University of California, Los Angeles and Baidu Research, and are licensed under a [Creative Commons Attribution 4.0 License](https://creativecommons.org/licenses/by/4.0/legalcode).