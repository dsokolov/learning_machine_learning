##Осваиваю tensorflow.

Создаём requirements.txt

`pip freeze > requirements.txt`

Создаём виртуальное окружение

`virtualenv -p python3.6 venv`

Запуск venv

`source ./venv/bin/activate`

Устанавливаем зависимости

`pip install -r requirements.txt`

Запуск jupyter-notebook

`venv/bin/python venv/bin/jupyter-notebook --no-browser --ip 127.0.0.1 --port 8888 --port-retries=0`

Экспортируем модель в tflite

`venv/bin/tflite_convert --saved_model_dir models/1551101184/ --output_file=model.lite`

###Tensorboard

Запуск tensorboard

`venv/bin/tensorboard --logdir tensorboard_logs/`

Остановить tensorboard

`pkill -f "tensorboard"`