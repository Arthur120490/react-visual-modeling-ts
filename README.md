# react-visual-modeling-ts
Адаптация библиотеки react-visual-modeling под react 17.0.2 + typescript 
 Feature
supports React 17.0.2
supports Typescript
npm install @vosdux/react-visual-modeling-ts
node - таблица edge - связь

Название	Описание	Тип
data	Данные для отрисовки	any
width	Ширина canvas	number | string
height	Высота canvas	number | string 
className	className	string
columns	Описание колонокcolumns props	Array<columns>
nodeMenu	Меню для node	Array<menu>
edgeMenu	Меню для edge	Array<menu>
actionMenu	Общее меню	action[]
config	Конфигурацияconfig props	any
emptyContent	Контент для пустой таблицы	string | JSX. Element
emptyWidth	Ширина пустой таблицы	number | string
beforeDeleteNode	Колбек удаления node	???
beforeDeleteEdge	Колбек удаления edge	???
onLoaded	Событие загрузки	(canvas) => void
onChange	Событие изменения (например добавление связи)	(data) => void
onFocusNode	Событие фокусировки на node	(node) => void
onFocusEdge	Событие фокусировки на edge	(edge) => void
onFocusCanvas	Событие фокусировки на canvas	() => void
onDblClickNode	Событие двойного клика на node	(node) => void
onDblClickEdge	Событие двойного клика на edge	(node) => void
selectable	???	boolean
onSelect	???	(nodes, edges) => void
columns
Название	Описание	Тип
title	Наименование	string
key	Ключ	string
width	Ширина	number
primaryKey	Первичный ключ	boolean
render	Рендер метод	(key) => void
menu
Название	Описание	Тип
title	Наименование	string
key	Ключ	string
render	Рендер метод	(key) => void
onClick	Клик	(key, data) => void
config
Название	Описание	Тип
disableDeleting	Отключить возможность удаления node	boolean
disableCollapse	Отключить возможность сворачивания node	boolean
disableEdgeCreation	Отключить возможность создавать связи в ручную	boolean
showActionIcon	Показать главное меню	boolean
allowKeyboard	Разрешить события с клавиатуры	boolean
titleRender	Рендер наменования node	(title) => JSX.Element
titleExtIconRender	Рендер иконки в шапке node	(node) => JSX.Element
labelRender	Рендер лейбла edge	(label) => JSX.Element
minimap	Настройки миникарты	minimap prop { }
autoLayout	Автоматическое позициониование	layout prop { }
gridMode	Настройки холста	grid prop { }
grid prop
Название	Описание	Тип
isAdsorb	???	boolean
theme	Настройки темы	theme prop { }
grid theme
Название	Описание	Тип
shapeType	Круги или линии	string
gap	Отступы	number
lineWidth	Ширина линии	boolean
lineColor	Цвет линии	string
circleRadiu	Радиус круга	number
circleColor	Цвет круга	string
layout prop
Название	Описание	Тип
type	https://github.com/alibaba/butterfly/blob/master/docs/en-US/layout.md	string
options	https://github.com/alibaba/butterfly/blob/master/docs/en-US/layout.md	any
minimap
Название	Описание	Тип
enable	Включить миникарту	boolean
config	Кофигурация	minimap props
minimap-config-prop
Название	Описание	Тип
nodeColor	Цвет ноды	string
activeNodeColor	Цвет активной ноды	string
viewportStyle	css стили - не CssProperties	Record<string, string>
