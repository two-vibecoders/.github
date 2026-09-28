# two-vibecoders

<p align="center">
  <img src="https://raw.githubusercontent.com/two-vibecoders/bus-cursor/master/assets/bus.svg" alt="Bus" width="120" height="120" />
</p>

<p align="center">
  <strong>Файловая шина агентов</strong><br/>
  одна идея — два скилла: Claude Code и Cursor IDE
</p>

<p align="center">
  <a href="https://two-vibecoders.github.io">Сайт</a>
  ·
  <a href="https://github.com/two-vibecoders/bus-claude">bus-claude</a>
  ·
  <a href="https://github.com/two-vibecoders/bus-cursor">bus-cursor</a>
</p>

---

## Проекты

Сообщения и задачи между агентами лежат во входящих, пока их не прочтут. Адресация по **имени**, типы `TASK` / `QUESTION` / `DONE`, веб-UI и фоновый подъём получателя.

| | [Bus Claude](https://github.com/two-vibecoders/bus-claude) | [Bus Cursor](https://github.com/two-vibecoders/bus-cursor) |
|---|---|---|
| Для | Claude Code | Cursor IDE |
| Скилл | `~/.claude/skills/bus` | `~/.cursor/skills/bus-cursor` |
| Движок | Claude Code | Cursor CLI (`agent -p`) |

Оба репозитория в этой организации. Основа шины — [jtapes/claude-bus](https://github.com/jtapes/claude-bus) ([JTapes](https://github.com/jtapes)); порт под Cursor и org — [SafonovAG](https://github.com/SafonovAG).

### Bus Claude

Скилл `bus` для Claude Code: файловая переписка агентов и локальный веб-UI.

```bash
# скопировать содержимое skills/bus → ~/.claude/skills/bus
```

Репозиторий: [two-vibecoders/bus-claude](https://github.com/two-vibecoders/bus-claude)

### Bus Cursor

Тот же подход для Cursor IDE: UI, фоновый подъём через Cursor CLI, расписание, настройки проекта.

```powershell
git clone https://github.com/two-vibecoders/bus-cursor.git "$env:USERPROFILE\.cursor\skills\bus-cursor"
& "$env:USERPROFILE\.cursor\skills\bus-cursor\install.ps1"
```

```bash
git clone https://github.com/two-vibecoders/bus-cursor.git ~/.cursor/skills/bus-cursor
~/.cursor/skills/bus-cursor/install.sh
```

Репозиторий: [two-vibecoders/bus-cursor](https://github.com/two-vibecoders/bus-cursor)

---

Сайт: [two-vibecoders.github.io](https://two-vibecoders.github.io)
