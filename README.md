# linearized_metrics_for_ABtest

Относительно недавно (в 2018-м году) исследователи из Яндекса разработали метод анализа тестов над метриками-отношениями вида 𝑥/𝑦.
Идея метода заключается в следующем:
Вместо того, чтобы использовать в статистичесих тестах "голые" метрики, можно сконструировать другую относительно рассматриваемой переменной метрику и анализировать ее.
* Считаем общий CTR в контрольной группе  𝐶𝑇𝑅𝑐𝑜𝑛𝑡𝑟𝑜𝑙=𝑠𝑢𝑚(𝑙𝑖𝑘𝑒𝑠)/𝑠𝑢𝑚(𝑣𝑖𝑒𝑤𝑠) 
* Посчитаем в обеих группах поюзерную метрику  𝑙𝑖𝑛𝑒𝑎𝑟𝑖𝑧𝑒𝑑_𝑙𝑖𝑘𝑒𝑠=𝑙𝑖𝑘𝑒𝑠−𝐶𝑇𝑅𝑐𝑜𝑛𝑡𝑟𝑜𝑙∗𝑣𝑖𝑒𝑤𝑠 
* После чего сравним  t-тестом отличия в группах по метрике 𝑙𝑖𝑛𝑒𝑎𝑟𝑖𝑧𝑒𝑑_𝑙𝑖𝑘𝑒𝑠

Чувствительность метрики увеличилась. Выводы в блокноте.

----
Relatively recently (in 2018), Yandex researchers have developed a method for analyzing tests on metrics-relations of the form x/y. The idea of the method is as follows: Instead
of using "naked" metrics in statistical tests, you can construct another metric relative to the variable under consideration and analyze it.

The sensitivity of the metric has increased. Conclusions in the notebook.
