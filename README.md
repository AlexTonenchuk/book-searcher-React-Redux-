Book-searcher.

Cоздано с ипользованием React, Redux, Redux-Toolkit.

Особенности проекта:

  - Управление состоянием осуществляется только из store, 
    созданного с использованием Redax-Toolkit
    (https://redux.js.org/introduction/getting-started#redux-toolkit);
    
  - Асинхронная логика написана с использованием Thunk
    (https://redux.js.org/tutorials/essentials/part-2-app-structure#writing-async-logic-with-thunks).
    

Для начала работы:

    - Book-searcher осуществляет поиск книг в Google Books APIs,
      для доступа к данным сервера Books APIs необхдимо получить ключ
      (https://developers.google.com/books/docs/v1/using);
    
    - Для авторизации запросов к API выбран способ с предоставлением API key 
      (https://developers.google.com/books/docs/v1/using#APIKey);
        
    - Скачайте Book-searcher;
    
    - Загрузите npm пакеты cmd: npm i;
    
    - Запустите проект на локальном хосте cmd: npm start.

Функционал:
    
    - По введенной пользователем подстроке производится поиск книг;
    
    - Фильтрация по категориям. Ниже текстового поля располагается селект с категориями: 
      all, art, biography, computers, history, medical, poetry. 
      Если выбрано "all" (выбрано изначально), то поиск производится по всем категориям;
    
    - Сортировка. Рядом с селектом категорий находится селект с вариантами сортировки: 
      relevance (выбран изначально), newest;
    
    - Найденные книги отображаются карточками, каждая из которых состоит из изображения обложки книги, 
      названия книги, названия категории и имен авторов. Если не приходит какой-либо части данных, 
      то вместо нее пустое место;
    
    - Над блоком с карточками отображается количество найденных по запросу книг;
    
    - Пагинация реализована по принципу 'load more'. Ниже блока с карточками находится 
      кнопка 'Load more', по клику на нее к уже загруженным книгам подгружаются еще. Шаг пагинации - 30;
    
    - При клике на карточку происходит переход на детальную страницу книги, на которой выводятся ее данные: 
      изображение обложки, название, категории, авторы, описание.

Внешний вид Book-searcher:

![image](https://user-images.githubusercontent.com/105805998/177460164-18da3130-8825-4e6b-9603-268420023052.png)



![image](https://user-images.githubusercontent.com/105805998/177460198-4101c346-0165-42d4-b26d-a3298c5a46ef.png)

