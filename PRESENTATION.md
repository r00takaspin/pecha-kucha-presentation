<!-- $theme: default -->
<!-- $size: 4:3 -->
![bg original](./images/intro.png)

--- 
![bg original](./images/bg.png)
# VUE.JS + RUBY ON RAILS = :heart:
## Правильный выбор Automatic View Library для Ruby on Rails приложений.

###### Вольдэмар Дулецкий ( [@r00takaspin](https://github.com/r00takaspin) ) 

---
![bg original](./images/bg.png)
# RUBY ON RAILS (RoR)
![](./images/ruby.png)
 :rocket: RoR позволяет быстро и качественно писать бэкэнд
 :pray: Ruby божественен, вызывает привыкание
 :skull: RoR имеет бедный View Layer

---
![bg original](./images/bg.png)
# VUE.JS
<img src="./images/vue-js.png" width="27%" />

:sunglasses: Прежде всего View библиотека, а не framework
:hammer: Компактен, быстр, прост
:zap: Очень похож на React: Virtual DOM, компоненты, Vuex

**Иногда сравнивают как смесь Angular 1 и React*.

---
![bg original](./iamges/bg.png)
# :fire: Rails 5.1
* **Webpack работает из коробки**
* Выпилен jQuery
* Выпилен Turbolinks


--- 
![bg original](./images/bg.png)
# :metal: Какие проблемы решаем?

--- 
![bg original](./images/bg.png)
# :punch: Избавляемся от мусора в бэкэнде
* удаляем лишние декораторы
* удаляем лишние хелперы для рендеринга HTML
* облегчаем контроллеры
---
![bg original](./images/bg.png)
# :punch: Работа со стейтом отдельных компонент без перезагрузки страниц

---
![bg original](./images/bg.png)
# :punch: Делегируем рендеринг Vue.js.
Фронтэнд лежит в отдельной папке с собственной структурой, собственными тестами и конфигами. Сюда переносим логику из декораторов и хелперов. 

---

# :eyes: Как выглядит компонент?
Отдельный файл c расширением .vue:
```html
<template>
Say hello: <span class='colored'>{{ $hello }} </span>
</template>
<style>
.colored {
  color: 'yellow'
}
</style>
<script>
export default {
  name: 'hello-component',
  data(): {
    return { hello: 'Hello, buddy' }
  },
  mounted() {
    console.log('hey, I am inited')
  }
}
</script>
```
---
![bg original](./images/bg.png)
# :electric_plug: Модульность
Через модули и миксины мы можем выносить общую логику в отдельные сущности и при необходимости их подключать.

---
![bg original](./images/bg.png)
# :dart: Trade-off

* Часть сайта можно делать как одностраничное приложение
* Часть приложения можно полностью рендерить без Vue.js
* При необходимости подключать компоненты для рендеринга части страницы
* Авторизацию оставим за Rails

---
![bg original](./images/bg.png)
# :coffee: А тесты?

Естественно всю логику которую мы вынесли из бэкэнда в компоненты мы покрываем тестами через святую троицу: `karma`, `jasmine`, `phantom-js`.

---
![bg original](./images/bg.png)
# :ru: Документация на русском языке
Вся документация по библиотекам входящим в экосистему есть на русском языке и поддерживается в актуально состоянии.

---
![bg original](./images/bg.png)
# <img src="./images/github.png" width="5%" /> Небольшое, отзывчивое комьюнити
:heavy_plus_sign: авторы библиотек отвечают быстро.
:heavy_minus_sign: документация не core-библиотек может не соответстовать актуально версии

---
![bg original](./images/bg.png)
<center><img src="./images/awesome-vue.png" width="60%" /></center>

* **vee-validations** - валидации
* **vue-resource** - годный http клиент
* **vue-i18n** - переводы
* **vue-router** - роутер для SPA

###### Полный список: awesome-vue.com

---
![bg original](./images/bg.png)
# :x:  Где не стоит использовать?
Гибридные приложения.

---
![bg original](./images/bg.png)
# :white_check_mark: Где стоит использовать?
Везде где нужна быстрая и функциональная View библиотека без лишних зависимостей.

---
![bg original](./images/bg.png)
# :wine_glass:  Хотите больше узнать о руби?
Приходите на koenig‐rb 7 апреля.

### :speech_balloon: Общаемся.
### :mortar_board: Показываем слайды.
### :beer:/:wine_glass: Выпиваем.

##### Сайт: koenig-rb.ru
---
![bg original](./images/bg.png)
# Контакты

<img src="./images/me.gif" width="40%" />

##### Вольдэмар Дулецкий

### https://github.com/r00takaspin
### https://fb.com/voldemar.duletskiy
voldemar.duletskiy@gmail.com

---
![bg original](./images/bg.png)
# <center>Вопросы?</center>