---
title: Шаблоны
contributors: [pavelgonzales]
outdated: true
---

Вы можете использовать [систему шаблонов](https://docs.nativescript.org/tooling/app-templates) для загрузки вашего `nativescript-vue` приложения. Все шаблоны генерируются с плагином nativescript-vue. Некоторые шаблоны имеют поддержку компонентов Vue.js (.vue) и livereload.

## nativescript-vue-template

#### Ссылка

[nativescript-vue-template](https://github.com/tralves/nativescript-vue-template)

#### Описание

Это самый базовый шаблон. Он имеет несколько примеров приложений с которых вы можете начать. Просто скопируйте и вставьте код из `app-with-list-view.js`, `app-with-router.js`, `app-with-tab-view.js` или `app-with-vmodel.js` в ваш `app.js`.

#### Установка

```shell
$ tns create sample-app --template nativescript-vue-template
```

*Для дальнейших инструкций перейдите по [ссылке](https://github.com/tralves/nativescript-vue-template).*

## nativescript-vue-rollup-template

#### Ссылка

[nativescript-vue-rollup-template](https://github.com/tralves/nativescript-vue-rollup-template)

#### Описание

Изначально это был форк от [rigor789](https://github.com/rigor789/nativescript-vue-rollup-template), в настоящее время это шаблон является самым стабильным и полнофункциональным. Посмотреть на него вы можете в приложении [🍏 🍍 🍓 Groceries Vue](https://github.com/tralves/groceries-ns-vue). Он поддерживает:

- livereload;
- Однофайловые компоненты .vue;
- scss импорты и scss внутри тэга `<style>` в комопненте .vue;
- корневой импорт (импорт начинается с корня приложения `/ `);
- babel с `es2015` и `stage-2` пресетами;

#### Установка

```shell
$ tns create sample-app --template nativescript-vue-rollup-template
```

*Для дальнейших инструкций перейдите по [ссылке](https://github.com/tralves/nativescript-vue-rollup-template).*

## nativescript-vue-webpack-template

#### Ссылка

[nativescript-vue-webpack-template](https://github.com/tralves/nativescript-vue-webpack-template)

#### Описание

Nativescript-vue-webpack-template использует webpack для обеспечения той же функциональности, что и rollup. Он поддерживает совместное использование нативного (android/iOS) и JavaScript кода.

<!-- The webpack template leverages webpack to provide the same functionality as the rollup counterpart. It is evolving to support code sharing, i.e., create projects that share as much of the logic as possible between a web build and the native (android/iOS) builds. -->

 Особенности:

- livereload;
- Однофайловые компоненты .vue;
- scss импорты и scss внутри тэга `<style>` в комопненте .vue;
- babel с `es2015` и `stage-2` пресетами;
- (скоро) совместное использование нативного и JavaScript кода;

#### Установка

```shell
$ tns create sample-app --template https://github.com/tralves/nativescript-vue-webpack-template
```

*Для дальнейших инструкций перейдите по [ссылке](https://github.com/tralves/nativescript-vue-webpack-template).*
