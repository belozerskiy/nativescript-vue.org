---
title: DockLayout
apiRef: https://docs.nativescript.org/api-reference/modules/_ui_layouts_dock_layout_
contributors: [pavelgonzales]
---

DockLayout позволяет размещать дочерние элементы относительно своих сторон (`left`, `right`, `top`, `bottom`) или центра используя механизм стыковки. Для определения стыковочной строны относительно DockLayout используйте свойство `dock` у дочернего элемента. Чтобы разместить элемент в центре DockLayout, он должен быть **последним дочерним элеменетом**, а у родителя свойство `stretchLastChild` должно быть `true`.

### Примеры

#### Элементы расположены с каждой стророны без растяжения последнего элемента

```html
<DockLayout stretchLastChild="false" backgroundColor="#3c495e">
  <Label text="left" dock="left" width="40" backgroundColor="#43b883"/>
  <Label text="top" dock="top" height="40" backgroundColor="#289062"/>
  <Label text="right" dock="right" width="40" backgroundColor="#43b883"/>
  <Label text="bottom" dock="bottom" height="40" backgroundColor="#289062"/>
</DockLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/dock_layout_no_stretch.svg" />

#### Элементы расположены с каждой стророны с растяжением последнего элемента

```html
<DockLayout stretchLastChild="true" backgroundColor="#3c495e">
  <Label text="left" dock="left" width="40" backgroundColor="#43b883"/>
  <Label text="top" dock="top" height="40" backgroundColor="#289062"/>
  <Label text="right" dock="right" width="40" backgroundColor="#43b883"/>
  <Label text="bottom" dock="bottom" backgroundColor="#1c6b48"/>
</DockLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/dock_layout_stretch.svg" />

#### Multiple children on the same side

```html
<DockLayout stretchLastChild="true" backgroundColor="#3c495e">
  <Label text="left 1" dock="left" width="40" backgroundColor="#43b883"/>
  <Label text="left 2" dock="left" width="40" backgroundColor="#289062"/>
  <Label text="left 3" dock="left" width="40" backgroundColor="#1c6b48"/>
  <Label text="last child" backgroundColor="#43b883"/>
</DockLayout>
```
<img class="md:w-1/2 lg:w-1/3" src="https://art.nativescript-vue.org/layouts/dock_layout_multiple_on_same_side.svg" />

## Входные параметры (Props)

| имя | тип | описание |
|------|------|-------------|
`stretchLastChild` | `Boolean` | Включает/Отключает растяжение последнего элемента на все свободное пространство.

## Входные параметры для дочерних элементов

У дочерних элементов первого уровня DockLayout появляются свойства:

| имя | тип | описание |
|------|------|-------------|
`dock` | `String` | Указывает к какой стороне пристыковать элемент: `top`, `right`, `bottom`, `left`
