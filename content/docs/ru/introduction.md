---
title: Введение
contributors: [rigor789, tjvantoll, belozerskiy]
---

## Что такое [NativeScript](https://www.nativescript.org/)?

NativeScript это фреймворк с открытым исходным кодом предназначенный для создания нативных мобильных приложений использующий javascript
<!-- NativeScript is an open source framework for building truly native mobile application using JavaScript.
 -->

## Что такое [Vue.js](https://vuejs.org/)?
Vue (произносится /vjuː/, примерно как view) — это прогрессивный фреймворк для создания пользовательских интерфейсов. В отличие от фреймворков-монолитов, Vue создан пригодным для постепенного внедрения. Его ядро в первую очередь решает задачи уровня представления (view), что упрощает интеграцию с другими библиотеками и существующими проектами.

## Что такое NativeScript-Vue?

NativeScript-Vue является плагином для NativeScript который позволяет вам использовать Vue.js для создания мобильных приложений. 
<!-- NativeScript-Vue is a NativeScript plugin which allows you to use Vue.js to craft your mobile application. -->

Если вы использовали Vue.js раньше вы почуствуете себя как дома с NativeScript-Vue. 
<!-- If you have used Vue.js before you will feel right at home with NativeScript-Vue. -->

## Зачем вам может понадобиться использовать это?

Существует множество возможностей создавать мобильные приложения. Здесь содержаться различные ситуации когда вам может пригодиться NativeScript-Vue 

<!-- There are many options to build mobile apps. Here are some situations where we think NativeScript-Vue is a great fit. -->

<!-- You need a truly native iOS and Android app -->
* **Вам необходимиы по настоящему нативные IOS и Android приложения**: NativeScript собирает ваши приложения используя нативные компрненты пользовательского интерфейса IOS и Andorid. Приложения которые вы создаете не являются Web приложениями, и поэтому они лишены ограничений связанных с WebView. NativeScript также предостовляет [внушительную коллекцию плагинов](http://market.nativescript.org/) которые позволяют использовать всевозможные фичи устройств. Так что если вам понадобиться связать IOS, Android API или прикрутить какую нибудь фичу как часть вашего приложения вы сможете сделать это при помощи NativeScript.  
<!-- builds your apps using native user interface components on iOS and Android. The apps you build are not web based, and therefore are not subject to the limitations inherent in WebView-based application frameworks. NativeScript also provides [an extensive collection of plugins](http://market.nativescript.org/) to tie into native device features. So if you need to tie into an iOS or Android API or feature as part of your app, you can do that with NativeScript. -->
<!-- You like JavaScript -->
* **Вам нравится JavaScript**: С NativeScript вы пишите код вашего мобильного приложения на JavaScript - не на Object-C, не на Swift и не на Java. Если вы любите JavaScript вы также полюбите писать нативные IOS и Android приложения на том же языке который вы используете в Web и/или в Node приложениях.   
<!-- With NativeScript you write your mobile applications in JavaScript — not Objective-C, not Swift, and not Java. If you like JavaScript, you’ll love writing native iOS and Android apps with the same language you use in your Web and/or Node apps. -->
<!-- You like Vue -->
* **Вам нравится Vue**: Vue известен своим простым подходом к управлению view слоем. Если вам нравится создавать веб приложения при помощи Vue, вы почуствуете себя как дома с NativeScript-Vue, используя тот-же синтаксис для решения общих задач таких как двунаправленное связывание(data binding) и обработка событий(event handling)
<!-- Vue is known for its simple approach to the view layer. If you like building web apps with Vue, you’ll be right at home with NativeScript-Vue, as you’ll be using the same syntax for handling common tasks like data binding and event handling. -->

<!-- ## What’s the catch? -->
## В чем прикол?

<!-- If you have existing Vue experience, there are two big things you’ll need to learn to be successful with NativeScript-Vue. -->
Если у вас уже есть опыт использования Vue, вам достаточно двух основных вещей для изучения чтобы быть успешным с NativeScript-Vue.


<!-- * **Working with the NativeScript CLI**: NativeScript is a framework for building iOS and Android apps, not web apps. You’ll need to learn how a few commands in the NativeScript CLI, and some basics of how iOS simulators and Android Virtual Devices work. -->
* **Работа с командной утилитой NativeScript CLI**: NativeScript это фремворк для создания IOS и Android приложений. Вам необходимо изучить руботу несколько команд в NativeScript CLI и некоторые основны работы с IOS и Android симулятором.
<!-- * **Learning the NativeScript UI components**: Because NativeScript uses native user interface components, HTML controls like `<div>` and `<span>` don’t exist in NativeScript. Instead you’ll need to learn a [new set of components](https://docs.nativescript.org/ui/components) you can use to render your interfaces. -->
* **Изучить UI компоненты NativeScript**: NativeScript использует компоненты нативных пользовательских интерфейсов, HTML теги такие как `<div>` и `<span>` не существет в NativeScript. Заместо них вам нужно использовать [новые компоненты](https://docs.nativescript.org/ui/components) для отрисовки вашего интерфейса.

<!-- Don’t worry though. Although there is a learning curve for working with NativeScript-Vue, you should find things much easier than learning iOS or Android from the ground up. After all, you’ll still be writing your source code in JavaScript and Vue. -->
Не волнуйтесь. Несмотря на то что здесь представлена кривая обучения для работы с NativeScript-Vue, вы поймете что некоторые вещи решаются легче чем изучение IOS и Androind  с нуля. И после всего, вы также сможете писать ваш код на JavaScript и Vue.

## Желаете поспособствовать?

NativeScript-Vue это проект с открытым исходным кодом и ???.
Загляни сюда [Гайд по Котрибуции](https://github.com/nativescript-vue/nativescript-vue/blob/master/CONTRIBUTING.md)
**Присоединяйтесь к нам в #vue канале [NativeScript Community Slack](https://developer.telerik.com/wp-login.php?action=slack-invitation)**.

## Насколько стабилен проект?

<!-- NativeScript-Vue is relatively feature complete. At this time we’re focusing on two things: -->
NativeScript-Vue относительно завершен. В данный момент мы сфокусированы на двух вещях:

<!-- * **Documentation**: Not everything you can do in NativeScript-Vue is documented on this site. We’re actively adding samples and use cases to this site, and contributions are welcome. -->
* **Документация**: Не все что вы можете сделать в NativeScript-Vue задокументировано. Мы активно добавляем примеры и полезные случаи использования, и нам бы непомешала помощь в этом от вас.
<!-- * **Sample apps**: We’re looking for people to put this plugin through its paces and send feedback our way. If you’re interested, join the [NativeScript Community Slack](https://developer.telerik.com/wp-login.php?action=slack-invitation) and let us know in the #vue channel. -->
* **Примеры приложений**: Мы ищем людей которые  We’re looking for people to put this plugin through its paces and send feedback our way. Если вы заинтересованы, присоединяйтесь к нам в слаке [NativeScript Community Slack](https://developer.telerik.com/wp-login.php?action=slack-invitation)
