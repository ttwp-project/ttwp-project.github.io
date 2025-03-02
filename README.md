# TTWP project by BerlandborAB 

# Что такое TTWP-project?

### **Text to Web Pages – превращаем текст в красивые веб-страницы**  

В мире, где информация правит балом, важна не только суть контента, но и его подача. **Text to Web Pages** – это легковесный статический сайт, который автоматически превращает текстовые файлы в красивые и удобные веб-страницы без необходимости в сервере или базе данных.  

📌 **Разворачивается за секунды на GitHub Pages** – просто загрузи файлы, и они моментально станут доступными онлайн!  

### 🔥 **Что умеет проект?**  
✅ **Автоматическая генерация страниц** – загрузи текстовый файл, и он превратится в полноценную статью.  
✅ **Поддержка Markdown** – используйте заголовки, списки, жирный/курсивный текст без HTML.  
✅ **Интерактивные ссылки** – поддержка YouTube, Google Drive, изображений, аудио и видео.  
✅ **Голосовое воспроизведение** – любой текст можно озвучить прямо на сайте.  
✅ **Lazy Loading** – статьи загружаются динамически, ускоряя загрузку сайта.  
✅ **SEO-оптимизация** – Open Graph и Twitter метатеги для красивого шаринга.  
✅ **Минимальные требования** – не требует серверов и баз данных, работает на GitHub Pages.  

### 🚀 **Кому подойдет?**  
- **Блогерам и авторам** – идеальный инструмент для публикации статей без CMS.  
- **Образовательным проектам** – удобный способ раздачи учебных материалов.  
- **Разработчикам** – быстрая альтернатива документации без серверного кода.  
- **Всем, кто хочет публиковать текст легко и быстро!**  

### 🎯 **Как это работает?**  
1️⃣ Загрузи текстовый файл в репозиторий GitHub.  
2️⃣ **Text to Web Pages** автоматически превращает его в интерактивную веб-страницу.  
3️⃣ Готово! Страница доступна через GitHub Pages, без настройки серверов и баз данных.  

📢 **Text to Web Pages – твой контент, готовый к публикации!** 🚀  

## Весь проект можно скачать здесь:

https://github.com/ttwp-project/ttwp-project.github.io/tree/main

## Подключения к html или локальная установка:

https://github.com/ttwp-project/ttwp-project.github.io/blob/main/styles.css 

https://ttwp-project.github.io/main/speech.js

https://ttwp-project.github.io/main/linkify.js

https://ttwp-project.github.io/main/CoreTTWP.js


    <script src="main/speech.js"></script>
    <script src="main/linkify.js"></script>
    <script src="main/CoreTTWP.js"></script



## основной html document 

```
<!DOCTYPE html>
<html lang="ru">
<head>



    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TTWP-project</title>
    <link rel="stylesheet" href="https://ttwp-project.github.io/styles.css">
</head>

<body>
    <h1>TTWP-project</h1>

    <!-- Оглавление (прокручиваемый блок) -->
    <div id="toc-container">
        <h2>Содержание</h2>
        <div id="toc"></div>
    </div><hr>


    
<div id="loadingIndicator" style="display: none; text-align: center; margin: 20px;">
    <div class="spinner"></div>
</div>

<!-- 🌟 Модальное окно настроек озвучки -->
<div id="speechModal" class="modal">
    <div class="modal-content">
        <span class="close" id="closeModal">&times;</span>
        <h2>Настройки озвучки</h2>
<p style="color: red;">Внимание! Озвучка работает только в браузере Chrome</p>

        <label for="languageSelect">Язык:</label>
        <select id="languageSelect"></select>

        <label for="voiceSelect">Голос:</label>
        <select id="voiceSelect"></select>

        <label for="rateInput">Скорость: <span id="rateValue">1</span></label>
        <input type="range" id="rateInput" min="0.5" max="2" step="0.1" value="1">

        <label for="pitchInput">Тональность: <span id="pitchValue">1</span></label>
        <input type="range" id="pitchInput" min="0.5" max="2" step="0.1" value="1">

        <button id="startSpeech">🔊 Начать озвучку</button>
        <button id="stopSpeech">⏹ Остановить</button>
    </div>
</div>



    <!-- Поле поиска -->
    <!-- Красивое поле поиска -->
<div class="search-container">
    <input type="text" id="searchInput" placeholder="Поиск по статьям..." oninput="searchPosts()">
</div>
    <div id="blog"></div>

    <!-- Кнопки для переключения страниц -->
    <div class="pagination">
        <button id="prevPage">← Назад</button>
        <span id="pageNumber">Страница 1</span>
        <button id="nextPage">Вперёд →</button>
    </div>
<p></p>

<p>© berlandbor</p>

    
    <script src="https://ttwp-project.github.io/main/speech.js
"></script>
    <script src=https://ttwp-project.github.io/main/linkify.js"></script>
    <script src="https://ttwp-project.github.io/main/CoreTTWP.js
"></script>

    <!--script src="script.js"></script-->
</body>
</html>


```


