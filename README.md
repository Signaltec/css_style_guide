# CSS style guide

## class или id
Всегда используйте class, даже если элемент один на странице.

## Отступы и пробелы
- Для отступов используйте двойной пробел. Если пользуетесь табуляцией —  правильно настройте свой текстовый редактор.
- Пробел между именем аттрибута и значением border: solid…

## Имена классов
Имена классов пишите в lowercase, через «-».

Неправильно:
```
.Item {}
.item_info {}
.itemInfo {}
```

Правильно:
```
.item {}
.item-info {}
```

## Как много классов нужно?
Как можно меньше, если есть элемент-контейнер, то внутренние элементы имеют класс, только по необходимости.

Неправильно:
```
<nav class="menu">
  <a class="menu-item" href=""></a>
  <a class="menu-item menu-item-selected" href=""></a>
  …
</nav>  
```

Правильно:
```
<nav class="menu">
  <a href=""></>
  <a class="selected" href=""></>
  …
</nav>  
```

## Краткая запись
Используйте краткую запись, если это возможно.

Неправильно:
```
  font-face: Arial;
  font-weight: bold;
  font-size: 12pt;
  border-style: solid;
  border-color: black;
  border-size: 1px;
```

Правильно:
```
  font: bold 12pt Arial;
  border: solid 1px black;
```

## Цвета
Используйте текстовые имена цветов и прозрачность.

Хорошо:
```
  color: MediumSeaGreen;
  border: solid 1px rgba(0,0,0,0.2);
```

## Таблицы или div
Используйте div, до тех пор пока это целесообразно.

## Float, flexbox
И то и то другое.

## CDN
Не используйте CDN. Все внешние классы должны быть включены в проект.

## CSS фреймворк
Используйте [http://npmjs.com/sega3](SEGA3).

## Препроцессоры
Мы используем less (пока).

## Порядок аттрибутов
Соблюдайте следующий порядок аттрибутов:
```
  display: block;
  position: absolute;

  margin: 1em 0;
  border: 20px solid black;

  background: green;
  box-shadow: 0 2px 10px #666;
  color: red;

  letter-spacing: 3px;
  font-size: 72px;
```

## Inline-стали
Мы используем inline-стили только для быстрого прототипирования. 
В рабочем проекте не должно быть inline-стилей.

## Инструменты
Мы используем CSScomb для того, чтобы наши css-файлы выглядили хорошо.








