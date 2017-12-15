# Поток событий для прецедента "Сделать ход"
## Основной поток
   
  1. Вариант использования начинается, когда пользователь, начав игру,
	   выбирает какой-либо игровой квадрат.
  2. Квадрат удаляется с игрового поля.
  3. Если цифра на квадрате меньше нужного числа, выполняется альтернативный поток А1.
  4. Приложение добавляет введенную сумму в базу данных согласно выбранному разделу.
  5. Вариант использование завершается.

## Альтернативный поток А1

  1. Пользоваетель выбирает ещё 1 квадрат и выполняется основной поток.
  2. Поток А1 завершается.

# Поток событий для прецедента "Пауза"
## Основной поток
   
  1. Вариант использования начинается, когда пользователь
	     нажимает на кнопку "Pause".
  2. Приложение выводит сообщение с предложением продолжить игру.
  3. Пользователь нажимая кнопку "Unpause" продолжает игру
  4. Вариант использование завершается.

# Поток событий для прецедента "Выход из игрового окна"
## Основной поток
   
  1. Вариант использования начинается, когда пользователь, находясь в окне игры,
	     нажимает на кнопку "Назад".
  2. Всплывает сообщение с выбором продолжения игры либо выхода в главное меню.
  3. При нажатии кнопки "No" пользователь продолжает игру.
  4. Пользователь нажимет кнопку "Yes" и выходит в главное меню.
  5. Вариант использование завершается.

# Поток событий для прецедента "Выход из игры"
## Основной поток
   
  1. Вариант использования начинается, когда пользователь, находясь в главном меню,
	   нажимает на кнопку "Назад".
  2. Всплывает сообщение, предлагающее нажать кнопку "Назад" ещё раз для выхода из игры.
  3. При повторном нажатии кнопки "Назад" пользователь выходит из игры.
  4 Вариант использование завершается.
## Альтернативный поток А1

  1. Приложение открывает экран детального отчета по выбранному разделу.
  2. Пользователь выбирает нужный пункт для его редактирования. 
  3. Приложение открывает экран для редактирования статьи расхода(дохода), суммы и/или даты.
  4. Пользователь изменяет данные при необходимости. В случае нажатия кнопки удаления 
	     выбранный пункт будет удален из истории.
  5. Поток А1 завершается.