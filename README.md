# gqa_lxmert

Download images from https://nlp.stanford.edu/data/gqa/images.zip and unzip to GQA_IMAGES_DIR

Run the following to get only the features for the testdev in ../hf_generated.datasets_testdev.datasets
```python extracting_data.py -i GQA_IMAGES_DIR -o hf_generated.datasets -t hf_generated.datasets_testdev.datasets -b BATCH_SIZE```

Run the following to get GQA dev set questions:
```wget https://nlp.stanford.edu/data/gqa/questions1.2.zip
unzip -j questions1.2.zip testdev_balanced_questions.json```

# Get features from the original LXMERT repo
```wget --no-check-certificate https://nlp1.cs.unc.edu/data/lxmert_data/vg_gqa_imgfeat/gqa_testdev_obj36.zip
unzip gqa_testdev_obj36.zip && rm gqa_testdev_obj36.zip```
