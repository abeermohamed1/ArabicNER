# ArabicNER

The winning solution to the [Topcoder Arabic NER challenge](https://www.topcoder.com/challenges/30087004).

# Environment setup

```
nvidia-docker build -t arabic_ner .
nvidia-docker run -v ``pwd''/data:/data:ro -v <Output Path>:/wdata -it arabic_ner
```

# Inference with pre-trained model

```
bash test.sh /data /wdata/solution.csv
```

# NER Model Training

```
bash train.sh /data
```

# Inference with trained NER model

```
bash test.sh /data /wdata/solution.csv
```

# Reference

Liyuan Liu, Jingbo Shang and Jiawei Han. “Arabic Named Entity Recognition: What Works and What’s Next” in Proc.of the 4th Arabic Natural Language Processing Worksho (WANLP 2019), co-located with ACL 2019, Florence, Italy, July2019.

