
# AB тестирование

- Реализовано различное отображение страницы в зависимости от GET параметра `ab-test-arg` который может принимать значения original и test.

- В отображении `app.views.index` реализован подсчет переходов с лендинга на основе GET параметра `from-landing` (на каждой из страниц лендинга
ссылка на главную страниц имеет вид `/?from-landing=original` и `/?from-landing=test`), если параметр не указан, такой случай не рассматривается как переход с лендинга

- В отображении `app.views.stats` реализован вывод отношения количества переходов к количеству показов страницы для обоих версий лендинга
