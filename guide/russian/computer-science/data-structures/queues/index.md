---
title: Queues
localeTitle: фрак
---
## Очереди

Очередь - структура данных First In First Out (FIFO). Многие алгоритмы используют очереди в своих ядрах для повышения производительности.

Очередь - один из основных абстрактных типов данных (ADT). Он похож на очереди, которые мы имеем в фильмах или супермаркетах. Первый человек, который должен прибыть, будет подан в первую очередь? Аналогично, первый элемент, который нужно вставить, будет удален первым. Существует несколько типов очередей, таких как,

1.  Простая очередь (или очередь)
2.  Круговая очередь
3.  Очередь приоритетов
4.  Dequeue (Double Ended Queue)

Если вы можете понять простую очередь (которая здесь будет упоминаться как «Очередь»), то все остальные будут такими же легкими, с небольшими изменениями.

Наиболее распространенными операциями, доступными в очереди, являются:

1.  Добавить / Предложение - Вставляет элемент в конец очереди.
2.  Удалить / Опрос. Удалите элемент с начала очереди.
3.  Peek - возвращает элемент в начале очереди, но не удаляет его.
4.  Size / Count - Возвращает количество элементов, присутствующих в очереди.
5.  IsEmpty - Проверьте, пуста ли очередь или нет.

Реализация очереди возможна с использованием массивов или связанных списков. Ниже приведена простая реализация массива структуры данных очереди с ее наиболее распространенными операциями.

\`\` \`JavaScript  
var Queue = function () { var queue = \[\]; var front = 0; var back = 0; вернуть { isEmpty: function () { return front> = назад || queue.length === 0; }, add: function (elem) { / \* Вы также можете сделать queue.push (elem) в JavaScript. Так они делают это на других языках \* / queue \[назад ++\] = elem; }, remove: function () { if (! this.isEmpty ()) { очередь возврата \[front ++\]; // или queue.shift () } else { throw new Error («Очередь пуста»); } }, peek: function () { if (! this.isEmpty ()) { очередь возврата \[фронт\]; } } } };

var queue = new Queue (); console.log (queue.isEmpty ()); // правда queue.add (1); queue.add (2); console.log (queue.remove ()); // 1 console.log (queue.peek ()); // 2 console.log (queue.remove ()); // 2 console.log (queue.remove ()); // исключение \`\` \`

#### Приложения

*   моделирование
*   Планирование (планирование работы, планирование диска)
*   Управление совместными ресурсами
*   Буфер клавиатуры
*   Поиск в ширину
*   Управлять перегрузками в сети

#### Дополнительная информация:

*   [Дополнительная информация о очередях - GeeksForGeeks](http://www.geeksforgeeks.org/queue-data-structure/)
*   [Решать проблемы с помощью очередей - Hackerrank](https://www.hackerrank.com/domains/data-structures/queues)
*   [HackerRank стеки и очереди видео](https://www.youtube.com/watch?v=wjI1WNcIntg)