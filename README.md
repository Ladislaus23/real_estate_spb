# Исследование рынка недвижимости Санкт-Петербурга и области

## Задача

Найти интересные особенности и зависимости, которые существуют на рынке недвижимости. Выполнить предобработку данных. 

## Данные

Имеется архив объявлений за несколько лет о продаже квартир в Санкт-Петербурге и соседних населённых пунктах. 

## Результаты исследования
Были обнаружены следующие интересные особенности:

- На рынке можно имеется большое предложение квартир с жилой площадью, меньше стандартной. Это может говорить о росте спроса на бюджетное жильё (квартиры-студии, малосемейки).
- Большая часть предложения представлена квартирами в хрущёвках (5 этажей) и в домах, построенных в позднесоветский период (9-10) этажей.
- Большая часть публикаций происходит в феврале-апреле и сентябре-октябре. По дням недели пик приходится на середину.
- Большая часть продаж происходит в первые 50-100 дней после публикации.

*Наиболее сильно стоимость жилья зависит от общей площади, менее всего на цену влияет дата публикации. Стоимость жилья растёт при уменьшении расстояния до центра.*

В таблицу были добавлены столбцы со следующей информацией: цена одного квадратного метра, день недели публикации объявления,
месяц публикации объявления, год публикации объявления, тип этажа квартиры, расстояние до центра города в километрах.

**В данных были обнаружены следующие проблемы:**

- Имеется большое количество пропусков в разных столбцах
- В большом количестве объявлений о продаже квартир за пределами Санкт-Петербурга, расстояние до центра города считается неверно (возникает большое число аномально высоких значений) 
- Неправильно считается или вообще отсутствует информация о расстояниях до ближайших парков и прудов.

Средние значения некоторых параметров:

- средняя стоимость объекта - 5 200 000
- средняя общая площадь - 54 м2
- в основном на рынке представлены 2-3 комнатные квартиры

Имеет смысл обратить внимание на бюджетный сегмент жилья (квартиры-студии) и элитный сегмент. Последние представлены в выборке меньше всего.


## Инструменты и навыки

Numpy, Pandas, Matplotlib, различные методы предобработки данных (заполнение пропусков, борьба с неявными дубликатами).
