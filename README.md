# Module_2_Babaina
Task of Module 2 Skillfactory
Задача проекта - провести разведовательный анализ данных по ученкаим с целью оценить влияние условий их жизни на успеваемость по математике
Цель проекта - дать рекомендации к построению модели для предсказания оценки на госэкзамене для всех учащихся
Этапы проекта:
1.Оценка качества данных
2.Очистка данных
3.Анализ неноминативных значений
4.Анализ номенативных значений
5.Выводы:
  -В данных достаточно мало пустых значений, только столбец Fedu был не заполнен более, чем в 10% случаев
  -Так же ключевой столбец score содержит в пределах 10% нулевых значений, которые похожи на выбросы
  -Выбросы также найдены столбцах Fedu & famrel. Большое количество выбросов в столбце absences.
  -Несмотря на то, что данные в столбце failures показывают статистически значимые различия, слишком большая доля всех данных приходится на значение 0. Но формулировка неоднозначна: 0 может означать как 0 неудач, так и больше 3 неудач - необходимо исследовать этот признак более подробно, прежде чем делать заключение о включении в модель
  -Отрицательная корреляция sudytime & studytime granular позволяет сделать вывод о том, что эти параметры представляют в разном формате одни и те же данные, для анализа оставляем только studytime
  -Самые важные параметры, которые предлагается использовать в дальнейшем для построения модели, это образование и профессия матери и отца (Medu, Fedu, Mjob, Fjob), адрес проживания (address), studytime, goout, schoolsup & failure (после доп.исследования параметра)
  -Также предлагается включить в анализ принадлежность к школе, пол, возраст (в качестве второстепенныхп араметров)
