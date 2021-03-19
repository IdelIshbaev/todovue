# todovue
## There no much style, but I have tried several features of vue.
#### 2 components used
#### ToDo can be added to the list
#### ToDo can be deleted from the list
#### ToDo can be marked as Done
#### ToDo list is saved in local storage and is not lost when page is updated
![Снимок экрана 2021-03-14 в 12 41 06](https://user-images.githubusercontent.com/41520293/111063966-93048180-84c2-11eb-98c8-e16433180ec6.png)

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


----------

Можно выполнить любое количество пунктов, цель задания: определить сильные и слабые стороны

[ ] исправить ошибки в hellowWorld.vue
 ### добавил :key=“item.id”, так как нужен dynamic binding
[ ] исправить ошибку в методе search
 ### Массив ничего не возвращал
[ ] улучшить алгоритм фильтрации (функция search)
 ### Добавил toLowerCase(), что в любом случае выдавался результат 
[ ] после фильтрации получить весь список, если ввести пустую строку
 ### done
[ ] фильтрация по нажатию enter внутри инпута
 ### по нажатию enter отправляю от компонента click, что является триггером для функции
[ ] Отрефакторить код (названия переменных, отступы, перенос кода, переименование файлов и т.д.)
 ### done
[ ] Написать стили для компонента (на свое усмотрение)
 ### Добавил вторую колонку, где результаты появляются сразу, без нажатия на кнопку или enter, можно скрыть эту колонку поставив галочку на checkbox.
 ### Еще добавил пару маленьких деталей
P.S. Не бойся выйти за рамки задания
 ### Добавил компонент loader, чтобы было красиво если дата долго фетчится, можно проверир с помощью setTimeOut() (App.vue, 26 строка)

[ ] решить проблему с типами
https://www.typescriptlang.org/play?#code/JYOwLgpgTgZghgYwgAgJICE4GcIBE5hzIDeAUMssACYBcyIArgLYBG0A3OcmMGADYQA-HSxgooAOacKwLAAlqVCCDosA9moFwQnAL6lSoSLEQpUAcShqGAB3yESXG3ACefNXFrIAglCiuAHgAlCAQ1KCoA0XEQCQAaZGjJAD5k6WRoKyhhZABRP3C9AyNoeCQ0S2sbDIAPSBAqLDRMHHsiMhksABlsMFUNLR0uKgI4HIsrWzai0jCQUWQmF0rbOgmq5ABeRxkvAFY4rlkFKiUVbigGCEPOntE6eD4cQ-1SGAYQBB41EGQARyuUBcAApnP4mHQQgDgFAIJF1rZkgBKHbIGAQMAIAAWwIA5N4AHIATQA+gBlXJBABqlJJuQJuAACgB5VAEgAquISHQoyHUVBcdAAUmTmQSAHRJWLAGAgsFwJjikaEJE3ZC6JGkV4A6AgpYrGxIzhAA

После решение вставить ссылку сюда:
---
https://www.typescriptlang.org/play?#code/JYOwLgpgTgZghgYwgAgJICE4GcIBE5hzIDeAUMssACYBcyIArgLYBG0A3OcmMGADYQA-HSxgooAOacKwLAAlqVCCDosA9moFwQnAL6lSoSLEQpUAcShqGAB3yESXG3ACefNXFrIAglCiuAHgAlCAQ1KCoA0XEQCQAaZGjJAD5k6WRoKyhhZABRP3C9AyNoeCQ0S2sbDIAPSBAqLDRMHHsiMhksABlsMFUNLR0uKgI4HIsrWzaigTBuCCY7UboJqrbkAF5HCmc3Dy8AbQBdUn0wkFFkJhdK203tyi8AVjiuWQUqJRVuKAYIV86PVEdHgfBwAOQI0IdEgizaEJ4-AgdAARCjTgYYAwQAgeGoQMgAI5-KAuAAUzn8TDoIWJwCgEEiq1syQAlA8YBAwAgABZkgDk3gAcgBNAD6AGVckEAGrSsW5IW4AAKAHlUEKACr8hIdCjIdRUFx0ABSEtVQoAdElYsAYOTKXAmJaoXBWRDdKyMQB6b0+MFqZA2NRYLDAFgCRKaBh4i6kX3Ic6Xa63Gw0ZnVLZkBMyZ6vHOUeSKZQw37-eN+wG9EFwMHlhP6BNYnGxokkh1wKkrVPs7OV5Cc7l8wWiyXSuVBBVKtUa7W6iv6iiG43IM0W61iSR2jtUl2jd0LiieheNv3N3HAfFt6A7p10bQuXuHgdc3kC4XiqWy+WKlXqrU6o4BZLmoRqmuaVo2hI24Up2Tp7oQB4FseDYGMSN5kimkw2KynBAA
---
