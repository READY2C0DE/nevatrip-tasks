1) Чтобы добавить дополнительные типы билета, нужно добавить по 2 столбца на каждый тип, где первый - цена билета по указанной категории, а второе это их количество по этой же категории(по аналогии с уже существующими типами билетов). Для добавления дополнительных типов следовать этому алгоритму.

2) Чтобы у каждогобилета в заказе был свой баркод, необходимо создать еще одну таблицу с колонками id, id_order, barcode, check_barcode. 
Где, id - инкрементальный порядковый номер билета, id_order - уникальный ид заказа(у каждого билета может быть только 1 номер заказа), barcode - уникальный штрих код билета, check_barcode - булевое значение, где 1 - посетитель прошел по этому баркоду, 0 - не прошел. Такая связь между таблицами называется один ко многим, так как у одного заказа может быть неограниченное множество билетов и соответсвенно barcode'ов к нему.

ps. Структуру таблицы передаю в 2-ух форматах(pdf и sql).