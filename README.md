### Описание функционала программы

Эта программа представляет собой инструмент для поиска утечек учетных данных (email и паролей) в базе данных, содержащей более 3.2 миллиардов записей. Она позволяет пользователям проверять, были ли их данные замечены в публичных утечках.

#### Основные функции:
1. **Проверка утечек данных**: Программа отправляет запрос к API с указанными данными (например, email или username) и получает результаты, если такие записи найдены.
2. **Графический интерфейс консоли**: Использует библиотеки `pystyle` и `colorama` для красивого отображения текста с цветовым оформлением.
3. **Безопасность использования**: Выводит предупреждение перед использованием, напоминая о необходимости соблюдать законность и этику.
4. **Многократный поиск**: Позволяет выполнять несколько поисков подряд без перезапуска программы.
5. **Чистый вывод**: После каждого поиска очищает консоль для лучшей читаемости.

---

### Предупреждение об использовании

> **ВАЖНОЕ ПРЕДУПРЕЖДЕНИЕ**
>
> Данная программа предназначена исключительно для образовательных целей. Использование данного программного обеспечения для незаконных действий строго запрещено. Автор не несет ответственности за любые неправомерные действия, совершенные с использованием этой программы. Продолжая использование, вы соглашаетесь с тем, что используете программу на свой страх и риск.
>
> Программа может быть использована только для проверки своих собственных данных или данных, на которые у вас есть разрешение владельца.

---

### Необходимые библиотеки

Перед запуском программы необходимо установить следующие библиотеки:

1. **`requests`** - Для работы с HTTP-запросами.
2. **`pystyle`** - Для создания стилей и эффектов текста в консоли.
3. **`colorama`** - Для работы с цветами в консоли.

#### Установка библиотек:

Вы можете установить все необходимые зависимости с помощью команды:

```bash
pip install requests pystyle colorama
```

---

### Инструкция по использованию

1. **Клонируйте репозиторий**:
   ```bash
   git clone https://github.com/broFR1K/AVVISPW.git
   cd AVVISPW
   ```

2. **Установите зависимости**:
   ```bash
   pip install requests pystyle colorama
   ```

3. **Запустите программу**:
   ```bash
   python main.py
   ```

4. **Введите данные для поиска**:
   - Программа попросит вас ввести email или другую информацию для проверки.
   - Если найдены соответствия, они будут выведены в формате:
     ```
     Пользователь: example@example.com
     Пароль: password123
     ```

5. **Повторный поиск**:
   - После завершения поиска программа предложит выполнить новый запрос или завершить работу.

---

### Пример работы

1. Запуск программы:
   ```
   $ python main.py
   ```

2. Отображение приветственного сообщения:
   ```
   ⚠️ ВНИМАНИЕ ⚠️
   Эта программа предназначена исключительно для образовательных целей.
   Использование данного программного обеспечения для незаконных действий строго запрещено.
   ...
   Нажмите Enter, чтобы продолжить...
   ```

3. Поиск данных:
   ```
   Введите данные для поиска: test@example.com

   Пользователь: test@example.com
   Пароль: mypassword123
   ------------------------------
   Хотите выполнить новый поиск? (y - да, n - нет): y
   ```

---

### Дополнительные замечания

- **API-ограничения**: Обратите внимание, что работа программы зависит от доступности внешнего API (`https://api.proxynova.com`). Если API недоступно, программа не сможет работать корректно.
- **Приватность**: Программа не хранит или передает ваши данные третьим лицам. Все запросы выполняются анонимно.

---

### GitHub README.md пример

```markdown
# Поисковик слитых паролей

## Описание
Эта программа позволяет проверять свои учетные данные на наличие в базах данных утечек. База содержит более 3.2 миллиардов записей.

## Предупреждение
⚠️ Данная программа предназначена исключительно для образовательных целей. Использование данного программного обеспечения для незаконных действий строго запрещено. Автор не несет ответственности за любые неправомерные действия, совершенные с использованием этой программы.

## Требования
- Python 3.6+
- Необходимые библиотеки:
  - `requests`
  - `pystyle`
  - `colorama`

## Установка
1. Клонируйте репозиторий:
   ```bash
   git clone https://github.com/broFR1K/AVVISPW.git
   cd AVVISPW
   ```
2. Установите зависимости:
   ```bash
   pip install requests pystyle colorama
   ```

## Запуск
```bash
python main.py
```

## Функционал
- Проверка утечек учетных данных.
- Графический интерфейс консоли с цветовым оформлением.
- Возможность многократного поиска без перезапуска программы.

## Пример работы
1. Запуск программы:
   ```
   $ python main.py
   ```
2. Отображение приветственного сообщения:
   ```
   ⚠️ ВНИМАНИЕ ⚠️
   Эта программа предназначена исключительно для образовательных целей.
   ...
   ```
3. Поиск данных:
   ```
   Введите данные для поиска: test@example.com

   Пользователь: test@example.com
   Пароль: mypassword123
   ------------------------------
   Хотите выполнить новый поиск? (y - да, n - нет): y
   ```




Такой README.md поможет пользователям легко понять, как использовать программу, и обратить внимание на важные моменты безопасности.
