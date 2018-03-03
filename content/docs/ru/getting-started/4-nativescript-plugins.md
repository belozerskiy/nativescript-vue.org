---
title: Использование NativeScript плагинов
contributors: [pavelgonzales]
---

Плагины работают так же, как и в любом другом приложении NativeScript, но вы можете задаться вопросом, как модули UI будут работать с Vue.

Использование UI плагинов очень похоже на использование NativeScript UI плагинов в Angular приложении. Рассмотрим пример использования [nativescript-gradient](https://github.com/EddyVerbruggen/nativescript-gradient), который используется в примере [listview sample](https://github.com/rigor789/nativescript-vue/tree/master/samples/app/app-with-list-view.js):

Установим плагин используя NativeScript CLI:

```shell
$ tns plugin add nativescript-gradient
```

Откройте входной файл вашего приложения и добавьте вверху:

```js
Vue.registerElement('Gradient', () => require('nativescript-gradient').Gradient)
```

Затем в вашем шаблоне вы можете использовать новый элемент:

```html
<Gradient direction="to right" colors="#FF0077, red, #FF00FF">
  <Label text="Best gradient." horizontalAlignment="center"
         style="color: white; padding: 20" />
</Gradient>
```
