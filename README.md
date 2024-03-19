# Практическая 4 - Генератор теста
Необходимо в приложении WPF реализовать генератор одного теста

# Необходимый функционал:
* Должно быть окно, где пользователь выбирает - пройти тест, или редактировать его
* Если пользователь хочет редактировать тест, ему нужно ввести кодовое слово (своего рода авторизация). Слово может быть любым. Как только он ввел слово, автоматически идет переход на авторизированное окно
* Редактор может переключаться между режимами - редактировать тест и пройти его, чтобы проверить на правильность
* Пользователь может только пройти тест. Редактор теста для него заблокирован
* После редактирования теста все данные должны быть сериализованы. При повторном открытии программы данные десериализуются и выгружаются в тест
* Вопрос в тесте должен обновляться согласно табличке в датагриде - пользователь нажал на вариант ответа, идет следующий вопрос. Данные выгружаются в текстовые поля и кнопки
* Если теста нет, тогда должна появиться соответствующая страница, в которой будет написано, что теста пока нет
* По окончанию теста должно отобразится на сколько правильных вопросов он ответил. Отображение правильного\неправильного ответа в течении теста не обязательно
* И редактор и пользователь должен иметь возможность вернуться обратно в окно авторизации
# Необходимая структура кода:
* Должно быть 2 окна - окно авторизации и авторизированное окно
* Должно быть 3 страницы - редактор теста, прохождение теста, отсутствие теста
* Переключение редактора между редакцией и прохождением теста должно происходить через страницы
* Тест должен быть моделью (своим типом) данных, состоящим из: названия, описания, 1, 2 и 3 вариант ответа, правильный ответ
* Правильный ответ должен быть представлен в виде Enum, не int
* Редактор теста должен быть в виде таблицы - DataGrid
* Верстка должна быть адаптивной. За невыполнение этого пункта минус 0,6 балла
* Кроме методов событий должны быть также реализованы отдельные приватные методы (весь код вы пишете не только в методах-событиях)

За каждый невыполненный пункт - минус 0,3 балла. Ниже 2 оценка быть не может