# Auditing a BERT-Based Toxicity Detector


## Background

```
● Growing online communities requires heavy moderation.
● Human moderators are fallible. Automated toxicity detectors are necessary for scale.
● Bias in these detectors can censor or fail to protect specific subgroups.
```


## BERT-Based Toxicity Detector

```
● 2,000,000 comments from Civil Commons tagged for toxicity.
    ○ Also tagged for Identity Groups
● Fine-tune a pre-trained BERT model for binary toxicity prediction.
● Evaluate using AUC-based metrics over different subgroups.
```


## Results on Test Set

```
● AUC for each subgroup displayed, as well as other slices of data.
● Fewer data and more societally targeted groups have lower performance.
● Performance across groups is relatively stable.
```

## SHAP Local Analysis: Don’t Say Gay?


## Conclusion

```
● The ADS performs well overall but struggles with the several protected groups.
● SHAP analysis reveals a failure to consider context, and bias against sensitive terms.
● ADS is useful to flag the worst content, the best method is human-in-the-loop.
```

