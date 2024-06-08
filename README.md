## GitHub Gist: Tmux Usage Guide



https://github.com/flaming-chameleon/tmux-short-guide/assets/73156836/72f62976-4102-4121-9458-dc0ddd263c45


[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)


### English Version

### Tmux: A Terminal Multiplexer

Tmux acts like a browser for your terminal, allowing you to create multiple sessions and switch between them easily within a single terminal window. One of its key features is that it keeps sessions running in the background, so you can reconnect from different devices without losing your work.

### Installation

![image](https://github.com/flaming-chameleon/tmux-short-guide/assets/73156836/188dcaeb-fa74-43c5-b791-3cfda89cc493)


#### Linux (Ubuntu):
```bash
sudo apt install tmux
```

#### MacOS (Homebrew):
```bash
brew install tmux
```

### Usage
![image](https://github.com/flaming-chameleon/tmux-short-guide/assets/73156836/0684f732-ba2a-4cbd-bf38-500edd0107b0)

#### Creating a Session
To create a new tmux session, use the following command:
```bash
tmux new -s bots
```
Here, `bots` is an example name for the session.

#### Running Multiple Bots
1. **Start the first bot:**
   ```bash
   cd ~/bots/bot1
   python main.py
   ```
2. **Create a new window for the second bot:**
   Press `Ctrl + b`, then press `c` to create a new window.
3. **Start the second bot:**
   ```bash
   cd ~/bots/bot2
   python main.py
   ```
4. Repeat these steps for all the bots you need to run.

### Essential Commands

#### Killing a Session
To delete a tmux session:
```bash
tmux kill-session -t (session_name)
```

#### Attaching to a Session
To reconnect to an existing session:
```bash
tmux a -t (session_name)
```

#### Listing Sessions
To list all tmux sessions:
```bash
tmux ls
```

### Key Combinations in Tmux

Inside tmux, key combinations are used by first pressing `Ctrl + b`, then the desired command.

- `c` - Create a new window
- `x` - Close the current window
- `w` - List all windows
- `d` - Detach from the session
- `0-9` - Switch to window number 0-9
- `p` or `n` - Switch to the previous or next window

### Additional Commands

- **Split Windows Horizontally:**
  ```bash
  Ctrl + b, %
  ```
- **Split Windows Vertically:**
  ```bash
  Ctrl + b, "
  ```
- **Navigate Between Panes:**
  ```bash
  Ctrl + b, arrow keys
  ```
- **Resize Panes:**
  ```bash
  Ctrl + b, Ctrl + arrow keys
  ```

By mastering these commands, you can efficiently manage multiple tasks and sessions within a single terminal window, making your development process more organized and productive.

---

### Russian Version

### Tmux: Мультиплексор Терминала

Tmux по сути является браузером для вашего терминала, позволяя создавать несколько сеансов и легко переключаться между ними в одном окне терминала. Одной из ключевых его особенностей является то, что он поддерживает сеансы постоянно включенными, так что вы можете переподключаться с различных устройств, не теряя свою работу.

### Установка

#### Linux (Ubuntu):
```bash
sudo apt install tmux
```

#### MacOS (Homebrew):
```bash
brew install tmux
```

### Использование

#### Создание Сессии
![image](https://github.com/flaming-chameleon/tmux-short-guide/assets/73156836/48229e5f-7f2e-4754-a614-55573d4687f1)

Чтобы создать новый сеанс tmux, используйте следующую команду:
```bash
tmux new -s bots
```
Здесь `bots` - это пример названия сеанса.

#### Запуск Нескольких Ботов
1. **Запустите первого бота:**
   ```bash
   cd ~/bots/bot1
   python main.py
   ```
2. **Создайте новое окно для второго бота:**
   Нажмите `Ctrl + b`, затем нажмите `c` для создания нового окна.
3. **Запустите второго бота:**
   ```bash
   cd ~/bots/bot2
   python main.py
   ```
4. Повторите эти шаги для всех необходимых ботов.

### Основные Команды

#### Удаление Сессии
Чтобы удалить сеанс tmux:
```bash
tmux kill-session -t (имя_сеанса)
```

#### Подключение к Сессии
Чтобы переподключиться к существующему сеансу:
```bash
tmux a -t (имя_сеанса)
```

#### Список Сеансов
Чтобы узнать имя всех сеансов tmux:
```bash
tmux ls
```

### Комбинации Клавиш в Tmux

Внутри tmux используются комбинации клавиш: сначала нажимаете `Ctrl + b`, затем нужную команду.

- `c` - создать новое окно
- `x` - закрыть текущее окно
- `w` - открыть список окон
- `d` - отключиться от сеанса
- `0-9` - переключение на окно номер 0-9
- `p` или `n` - переключение на предыдущее или следующее окно

### Дополнительные Команды

- **Разделить окно горизонтально:**
  ```bash
  Ctrl + b, %
  ```
- **Разделить окно вертикально:**
  ```bash
  Ctrl + b, "
  ```
- **Навигация между панелями:**
  ```bash
  Ctrl + b, стрелки
  ```
- **Изменение размера панелей:**
  ```bash
  Ctrl + b, Ctrl + стрелки
  ```

Освоив эти команды, вы сможете эффективно управлять несколькими задачами и сеансами в одном окне терминала, делая процесс разработки более организованным и продуктивным.

[![Join our Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/hidden_coding)
