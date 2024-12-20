# Сегментация новостных видеовыпусков
Обучение Bert-BiLSTM для сегментации транскриптов новостей по статье [Ghinassi et al., 2023](https://peerj.com/articles/cs-1593/)

## Части проекта:

### 1. Обучение модели сегментации текста 
*НОУТБУК:* [BiLSTM_topic_segmentation_train_eval.ipynb](https://githubtocolab.com/tony-pitchblack/news-segmentation/blob/main/BiLSTM_topic_segmentation_train_eval.ipynb)

Обучение модели с использованием исправленного и дополненного кода авторов статьи [NSE-TopicSegmentation](https://github.com/tony-pitchblack/NSE-TopicSegmentation)

Метрики на in-distribution тесте:

[<img src="https://github.com/tony-pitchblack/news-segmentation/blob/main/bert_bilstm_in_distribution_metrics.png" alt="In-distribution metrics" width="400"/>]()

### 2. Тестирование модели сегментации текста
*НОУТБУК*: [news_segmentation_ntv_eval.ipynb](https://githubtocolab.com/tony-pitchblack/news-segmentation/blob/main/BiLSTM_topic_segmentation_train_eval.ipynb)

Метрики на out-of-distribution тесте:

[<img src="https://github.com/tony-pitchblack/news-segmentation/blob/main/bert_bilstm_out_of_distribution_metrics.png" alt="In-distribution metrics" width="400"/>]()

*Пример вывода модели:*

[<img src="https://github.com/tony-pitchblack/news-segmentation/blob/main/bert_bilstm_example_output_ntv.png" alt="Out-of-distribution metrics" width="500"/>]()

### 3. Пайплайн Speech recognition + Text segmentation
*НОУТБУК:* [news_transcripts_topic_segmentation_demo.ipynb](https://colab.research.google.com/github/tony-pitchblack/news-segmentation/blob/main/news_transcripts_topic_segmentation_demo.ipynb)

* использование предобученной модели Whisper для распознавания речи
* сегментация транскрибированного текста с помощью обученной модели
