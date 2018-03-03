---
title: Использование Vue плагинов
contributors: [pavelgonzales]
---

## vue-router

Скоро...

## Vuex

Vuex это библиотека управления состоянием в Vue. Он служит хранилищем для данных и гарантирует предсказуемое измненение состояния приложения. Vuex может использоваться в NativeScript приложениях; для примера обратите внимание на [NativeScript Groceries Vue sample](https://github.com/tralves/groceries-ns-vue). 

### Установка

Установка Vuex производится так же, как и для простого Vue приложения

```shell
$ npm install vuex --save
```

Последняя версия Vuex будет добавлена в ваш package.json.

### Импорт

Вверху вашего `main.js`:

```js
import Vuex from 'vuex'
Vue.use(Vuex)
```

Теперь вы можете использовать Vuex аналогично тому, как вы использовали его в стандартном приложении Vue.

### Создание стора

В папке `/store` создадим константу с нашим стором. Простой стор включает в себя состояние счетчика и мутации изменяющие наше состояние:

```js
const store = new Vuex.Store({
    state: {
      count: 0
    },
    mutations: {
      increment: state => state.count++,
      decrement: state => state.count--
    }
})
```

### Использование стора

Теперь мы можем управлять нашим состоянием. В примере ниже мы создаем вычисляемое свойство `count` и изменяем его по нажатию на кнопку '+' или '-'. Обратите внимание что вы не изменяете ваше состояние напряую, а вызываете мутации которые это делают.

```js
new Vue({
  computed: {
    count(){
      return store.state.count
    }
  },

  template: `
    <Page>
      <ScrollView>
        <StackLayout>
          <Button @tap="increment" text="+" />
          <Button @tap="decrement" text="-" />
          <Label :text="count" />
        </StackLayout>
      </ScrollView>
    </Page>
  `,

  methods: {
    increment() {
      store.commit('increment')
    },
    decrement() {
      store.commit('decrement')
    }
  }
}).$start()
```

Больше информации о Vuex и об управлении состоянием вы найдете в [документации](https://vuex.vuejs.org/ru/). Хорошую архитектуру для управления различными элементами вы можете найти в приложении Groceries в [папке `/store`](https://github.com/tralves/groceries-ns-vue/tree/master/app/store).