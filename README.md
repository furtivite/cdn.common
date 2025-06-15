# cdn.common

cdn.common — это центральный репозиторий для хранения и публикации общих статических ресурсов через CDN, используемых в разных проектах вашей организации.

## 📁 Структура репозитория

cdn.common/

```
└── marketplace/      // Статические файлы (изображения, скрипты, стили) для проекта Marketplace
    ├── css/
    ├── js/
    └── images/
```


Примечание: На данный момент единственный каталог — marketplace.

## 🚀 Использование CDN

Мы используем jsDelivr для обёртки GitHub-репозитория и доставки файлов через глобальный CDN.

Шаблон URL:

```
https://cdn.jsdelivr.net/gh/<GitHub-username>/cdn.common@<тег или коммит>/<путь>/<до_файла>
```


Примеры
	•	Подключение CSS-файла:
	```
	<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/<GitHub-username>/cdn.common@main/marketplace/css/styles.css" />
	```
 
	•	Подключение JavaScript:
	```
	<script src="https://cdn.jsdelivr.net/gh/<GitHub-username>/cdn.common@v1.2.0/marketplace/js/app.js"></script>
	```

	•	Использование изображения:
	```
	<img src="https://cdn.jsdelivr.net/gh/<GitHub-username>/cdn.common@main/marketplace/images/logo.png" alt="Marketplace Logo" />
	```


## 🏷️ Теги и версии
	•	main — ветка для разработки стабильного релиза.
	•	vX.Y.Z — семантические теги для конкретных версий. При выпуске новой версии создавайте тег в формате v<major>.<minor>.<patch> и обновляйте ссылки.

## 🔄 Обновление содержимого

	1.	Вносите изменения в папку marketplace.
	2.	Делаете коммит и пуш в ветку main.
	3.	Опционально: создайте и запушьте тег для новой версии:

	  ```
    git tag v<новая-версия>
    git push origin v<новая-версия>
    ```
	4.	Ваши изменения сразу станут доступны по CDN-URL.

## 🤝 Contributing
	1.	Форкните репозиторий.
	2.	Создайте новую ветку:

`git checkout -b feature/your-feature`


	3.	Внесите правки и закоммитьте изменения.
	4.	Откройте Pull Request в основной репозиторий.

Пожалуйста, следуйте конвенциям именования файлов и придерживайтесь семантического версионирования.

## ⚖️ Лицензия

Этот проект распространяется под лицензией MIT. Смотрите файл LICENSE для деталей.
