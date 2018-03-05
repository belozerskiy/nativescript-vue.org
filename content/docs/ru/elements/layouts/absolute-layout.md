---
title: AbsoluteLayout
apiRef: https://docs.nativescript.org/api-reference/modules/_ui_layouts_absolute_layout_
contributors: [pavelgonzales]
---

AbsoluteLayout является самым простым лэйаут контейнером в NativeScript. Он использует абсолютные координаты для дочерних элементов. AbsoluteLayout не накладывает ограничений по размерам для дочерних элементов и не будет их изменять при изменении собственных размеров.

### Примеры

#### Сетка

```html
<AbsoluteLayout backgroundColor="#3c495e">
  <Label text="10,10" left="10" top="10" width="100" height="100" backgroundColor="#43b883"/>
  <Label text="120,10" left="120" top="10" width="100" height="100" backgroundColor="#43b883"/>
  <Label text="10,120" left="10" top="120" width="100" height="100" backgroundColor="#43b883"/>
  <Label text="120,120" left="120" top="120" width="100" height="100" backgroundColor="#43b883"/>
</AbsoluteLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/absolute_layout_grid.svg" />

#### Перекрывающие элементы

```html
<AbsoluteLayout backgroundColor="#3c495e">
  <Label text="10,10" left="10" top="10" width="100" height="100" backgroundColor="#289062"/>
  <Label text="30,40" left="30" top="40" width="100" height="100" backgroundColor="#43b883"/>
</AbsoluteLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/absolute_layout_overlap.svg" />


## Входные параметры (Props)

AbsoluteLayout не имеет входных параметров.

## Входные параметры для дочерних элементов

У дочерних элементов первого уровня AbsoluteLayout появляются свойства:

| имя | тип | описание |
|------|------|-------------|
| `top` | `Number` | Значение указывающее расстояние от верхнего края родиельского элемента AbsoluteLayout
| `left` | `Number` | Значение указывающее расстояние от левого края родиельского элемента AbsoluteLayout
