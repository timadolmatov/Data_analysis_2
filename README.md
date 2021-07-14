Целью данного проекта является: установить, какие параметры влияют на стоимость квартиры. Так же система, которую мы построим в ходе проекта будет сможет отслеживать аномалии и мошенеческую деятельность.

# Данные

В вашем распоряжении данные сервиса Яндекс.Недвижимость — архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет:

- airports_nearest — расстояние до ближайшего аэропорта в метрах (м)
- balcony — число балконов
- ceiling_height — высота потолков (м)
- cityCenters_nearest — расстояние до центра города (м)
- days_exposition — сколько дней было размещено объявление (от публикации до снятия)
- first_day_exposition — дата публикации
- floor — этаж
- floors_total — всего этажей в доме
- is_apartment — апартаменты (булев тип)
- kitchen_area — площадь кухни в квадратных метрах (м²)
- last_price — цена на момент снятия с публикации
- living_area — жилая площадь в квадратных метрах(м²)
- locality_name — название населённого пункта
- open_plan — свободная планировка (булев тип)
- parks_around3000 — число парков в радиусе 3 км
- parks_nearest — расстояние до ближайшего парка (м)
- ponds_around3000 — число водоёмов в радиусе 3 км
- ponds_nearest — расстояние до ближайшего водоёма (м)
- rooms — число комнат
- studio — квартира-студия (булев тип)
- total_area — площадь квартиры в квадратных метрах (м²)
- total_images — число фотографий квартиры в объявлении
----------------------------------------
3. **ОСНОВНЫЕ ПУНКТЫ И ЦЕЛИ ИССЛЕДОВАНИЯ:**
- Предобрботка данных:
  - определение и изучение пропущенных значений:
  - привести данные к нужным типам.
- Посчитать и добавить в таблицу:
  - цену квадратного метра;
  - день недели, месяц и год публикации объявления;
  - этаж квартиры; варианты — первый, последний, другой;
  - соотношение жилой и общей площади, а также отношение площади кухни к общей.
- Провести исследовательский анализ данных:
  - изучить параметры и построить для них гистограммы;
  - уберать редкие и выбивающиеся значения. Описать, какие особенности обнаружили;
  - какие факторы больше всего влияют на стоимость квартиры? Изучить, зависит ли цена от площади, числа комнат, удалённости от центра. Изучить зависимость цены от того, на каком этаже расположена квартира: первом, последнем или другом. Также изучить зависимость от даты размещения: дня недели, месяца и года;
  - выбрать 10 населённых пунктов с наибольшим числом объявлений. Посчитать среднюю цену квадратного метра в этих населённых пунктах. Выделить среди них населённые пункты с самой высокой и низкой стоимостью жилья. Эти данные можно найти по имени в столбце 'locality_name';
  - изучить предложения квартир. **Задача**: выяснить, какая область входит в центр. Создать столбец с расстоянием до центра в километрах: округлить до целых значений. После этого посчитайть среднюю цену для каждого километра. Построить график: он должен показывать, как цена зависит от удалённости от центра. Определить границу, где график сильно меняется — это и будет центральная зона;
  - выделить сегмент квартир в центре. Проанализировать эту территорию и изучите следующие параметры: площадь, цена, число комнат, высота потолков. Также выделить факторы, которые влияют на стоимость квартиры (число комнат, этаж, удалённость от центра, дата размещения объявления). Сделать выводы. Отличаются ли они от общих выводов по всему городу?
----------------------------------------
4. **ИСПОЛЬЗУЮЕМЫЕ БИБЛИОТЕКИ:**
- Pandas
- datetime
- IPython.display
- matplotlib.pyplot
