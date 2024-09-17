<DataBase>



0.1 Это проект по созданию своей библиотеки для работы с базами данных на Python,
библиотека может включать функции для создания, чтения, обновления и удаления данных (CRUD).



0.2 Название функций в библиотеке, в далнейшем времени сдесь появится больше функция и задач

from (Название мой библиотеки 'Она ещё в процесе разработки') import Database

# Создание базы данных и таблицы
db = Database('example.db')

# Структура таблицы
columns = {
    'id': 'INTEGER PRIMARY KEY AUTOINCREMENT',
    'name': 'TEXT',
    'age': 'INTEGER'
}

# Создание таблицы
db.create_table('users', columns)

# Вставка данных
db.insert('users', (None, 'Alice', 30))
db.insert('users', (None, 'Bob', 25))

# Получение и вывод всех данных
users = db.fetch_all('users')
print(users)

# Обновление данных
db.update('users', {'age': 31}, 'name = "Alice"')

# Удаление данных
db.delete('users', 'name = "Bob"')

# Закрытие программы
db.close()



0.3 В этом пункте появится способ установки моей библиотеки





KAPUSTA1651
