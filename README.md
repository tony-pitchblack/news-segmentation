# Сегментация новостных видеовыпусков
Обучение Bert-BiLSTM для сегментации транскриптов новостей по статье [Ghinassi et al., 2023](https://peerj.com/articles/cs-1593/)

## Части проекта:

### 1. Обучение модели сегментирования текста 
*НОУТБУК:* [BiLSTM_topic_segmentation_train_eval.ipynb](https://githubtocolab.com/tony-pitchblack/news-segmentation/blob/main/BiLSTM_topic_segmentation_train_eval.ipynb)

Обучение модели с использованием исправленного и дополненный кода авторов статьи [NSE-TopicSegmentation](https://github.com/tony-pitchblack/NSE-TopicSegmentation)

### 2. Пайплайн Speech recognition + Text segmentation
*НОУТБУК:* [news_transcripts_topic_segmentation_demo.ipynb](https://colab.research.google.com/github/tony-pitchblack/news-segmentation/blob/main/news_transcripts_topic_segmentation_demo.ipynb)

* использование предобученной модели Whisper для распознавания речи
* сегментация транскрибированного текста с помощью обученной модели
