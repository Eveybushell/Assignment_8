# Assignment_8
## by Evelyn Bushell

## Model
lora-distilbert-imdb

## Task
Classification of sentiment based on imdb reviews of films

## Metrics table
| Class | Precision | Recall | F1 | Accuracy |
|-------|-----------|--------|----|----------|
| Positive | 0.92 | 0.89 | 0.91 | 0.91 |
| Negative | 0.89 | 0.93 | 0.91 | 0.91 |

## F1 score vs Accuracy
F1 score tends to be a better metric for real life applications because it is more appropriate for imbalanced datasets. There is very little data in real life that is completely balanced. By using both recall and precision in its calculations, F1 is more reliable than accuracy which, depending on the dataset, could read as artificially high by predicting the majority class every time.

## Error Analysis
The model had a harder time identifying negative reviews. Looking at the two samples it pulled, it appears to be because people can find something they can enjoy in an otherwise disliked film. Whether this is returning to a once-loved film to find it aging poorly or a movie that is so-bad-it's-good in its cheesiness, there tends to be a lot of normally positive words mixed in with negative ones. 