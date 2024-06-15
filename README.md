# Сегментация новостных видеовыпусков
Чтобы просмотреть .ipynb файл в Google Colab, необходимо изменить его url адрес, добавив `tocolab` после `github`. 
Например: https://githubtocolab.com/tony-pitchblack/news-segmentation/blob/main/Insightface_demo.ipynb

Ссылки на статьи и другие материалы, полезные для проекта собраны в [Google Docs](https://docs.google.com/document/d/16adhUd1MXhHQTqz3p6X_Yth9nqWHLLruIYvZpRau1kc/edit?usp=sharing)


## Части проекта:
### 1. Face recognition on video
*ФАЙЛ:* Insightface_demo.ipynb

*ОПИСАНИЕ:* использование предобученной модели проекта Insightface для распознавания лиц на видео

### 2. Обучение модели сегментирования текста 
*ФАЙЛ:* BiLSTM_topic_segmentation_train_eval.ipynb

*ОПИСАНИЕ:* использование [форка пайплайна обучения моделей](https://github.com/tony-pitchblack/NSE-TopicSegmentation)  \
автора [статьи](https://peerj.com/articles/cs-1593/) для обучения BiLSTM


### 3. Пайплайн Speech recognition + Text segmentation
*ФАЙЛ:* news_transcripts_topic_segmentation_demo.ipynb

*ОПИСАНИЕ:* использование предобученной модели с huggingface для распознавания речи, \
а затем разбиение транскрибированного текста с помощью обученной BiLSTM, чекпоинт которой загружается с wandb
