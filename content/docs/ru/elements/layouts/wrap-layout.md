---
title: WrapLayout
apiRef: https://docs.nativescript.org/api-reference/modules/_ui_layouts_wrap_layout_
contributors: [pavelgonzales]
---

The WrapLayout container positions its children in rows or columns, based on the orientation property, until the space is filled and then wraps them onto a new row or column.

WrapLayout размещает свои дочерние элементы в строки или колонки базирующихся на свойстве `orientation`. Когда все пространство заполнено, WrapLayout переносит дочерние элементы на новую строку или колонку.

### Примеры

#### WrapLayout по умолчанию

```html
<WrapLayout backgroundColor="#3c495e">
  <Label text="first" width="30%" height="30%" backgroundColor="#43b883"/>
  <Label text="second" width="30%" height="30%" backgroundColor="#1c6b48"/>
  <Label text="third" width="30%" height="30%" backgroundColor="#289062"/>
  <Label text="fourth" width="30%" height="30%" backgroundColor="#289062"/>
</WrapLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/wrap_layout_horizontal.svg" />

#### WrapLayout с вертикальной ориентацией

```html
<WrapLayout orientation="vertical" backgroundColor="#3c495e">
  <Label text="first" width="30%" height="30%" backgroundColor="#43b883"/>
  <Label text="second" width="30%" height="30%" backgroundColor="#1c6b48"/>
  <Label text="third" width="30%" height="30%" backgroundColor="#289062"/>
  <Label text="fourth" width="30%" height="30%" backgroundColor="#289062"/>
</WrapLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/wrap_layout_vertical.svg" />

## Входные параметры (Props)

| имя | тип | описание |
|------|------|-------------|
`orientation` | `String` | Указывает направление потока. Если ориентация выставлена `horizontal`, то дочерние элементы располагаются в ряд. Если ориентация выставлена `vertical`, то дочерние элементы располагаются в колонку. По умолчанию стоит значение `horizontal`.
`itemWidth` | `Number` | Ограничивает ширину дочерних элементов. По умолчанию стоит значение `Number.NaN`, которое не ограничивает ширину дочерних элементов.
`itemHeight` | `Number` | Ограничивает высоту дочерних элементов. По умолчанию стоит значение `Number.NaN`, которое не ограничивает высоту дочерних элементов.

## Входные параметры для дочерних элементов

У дочерних элементов нет входных параметров.
