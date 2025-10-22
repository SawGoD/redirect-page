# ➡️ Страница перенаправления

Простая страница перенаправления, которая позволяет перенаправлять пользователей на другие URL-адреса с задержкой.

### 🧠 Что это такое?

Telegram Desktop на Windows некорректно открывает **внешние глубокие ссылки** (такие как `v2box://`, `happ://`, `clash://...` и т.д.), когда они приходят из браузера или сообщения.

## Использование

Добавьте параметр `redirect_to` к URL страницы:

```
https://sawgod.github.io/redirect-page/?redirect_to=clash://install-config?url=SUB_URL
```

### 🎨 Темы оформления

Вы можете выбрать тему оформления с помощью параметра `theme`:

```
https://sawgod.github.io/redirect-page/?theme=THEME_NAME&redirect_to=YOUR_URL
```

**Доступные темы:**
- `telegram` - Стандартная тема (используется по умолчанию, если тема не указана)
- `soft` - Мягкая розово-фиолетовая тема с карточками
- `simple` - Простая монохромная тема
- `minimal` - Минималистичная тема
- `retro` - Ретро-стиль с анимациями
- `apple` - Стиль Apple
- `google` - Стиль Google

**Примеры:**

```
# Стандартная тема (Telegram) - тему указывать не нужно
https://sawgod.github.io/redirect-page/?redirect_to=YOUR_URL

# Тема Soft
https://sawgod.github.io/redirect-page/?theme=soft&redirect_to=YOUR_URL

# Ретро тема
https://sawgod.github.io/redirect-page/?theme=retro&redirect_to=YOUR_URL
```

## Особенности

- ⏱️ Автоматическое перенаправление через 7 секунд
- 🔄 Кнопка для немедленного перенаправления
- 📱 Адаптивный дизайн (мобильные устройства и десктоп)
- 🌐 Автоматическое определение языка (русский/английский)
- 🌙 Поддержка темной темы
- 🔗 Отображение URL назначения

## Превью тем

<details>
  <summary>Стандартная/Telegram</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/telegram_light.png)  |  ![](img//telegram_dark.png)
</details>

<details>
  <summary>Ретро</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/retro_light.png)  |  ![](img/retro_dark.png)
</details>

<details>
  <summary>Soft</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/preview_light.png)  |  ![](img/preview_dark.png)
</details>

<details>
  <summary>Простая</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/simple_light.png)  |  ![](img/simple_dark.png)
</details>

<details>
  <summary>Минимальная</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/minimal_light.png)  |  ![](img/minimal_dark.png)
</details>

<details>
  <summary>Системные</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/apple_light.png)  |  ![](img/apple_dark.png)
![](img/google_light.png)  |  ![](img/google_dark.png)
</details>

---
## 🔧 Создание своей темы

Вы можете создать собственную тему для страницы перенаправления:

### Шаг 1: Создайте файл темы
Скопируйте `themes/template.html` (шаблон с подробными комментариями) или любую существующую тему в `themes/your-theme-name.html`

### Шаг 2: Настройте стили
Измените CSS в секции `<style>` под свой дизайн. Важно:
- Сохраните все ID элементов (они используются JavaScript)
- Добавьте поддержку тёмной темы через `@media (prefers-color-scheme: dark)`
- Сделайте дизайн адаптивным для мобильных устройств

### Шаг 3: Используйте свою тему
```
https://sawgod.github.io/redirect-page/?theme=your-theme-name&redirect_to=YOUR_URL
```

**Обязательные элементы (ID):**
- `title` - Заголовок страницы
- `subtitle` - Подзаголовок
- `timer` - Счётчик обратного отсчёта
- `redirectLink` - Кнопка перенаправления
- `url-display` - Отображение URL назначения

**Требуемый функционал:**
- 7-секундный таймер обратного отсчёта
- Поддержка параметра `redirect_to` из URL
- Двуязычная поддержка (русский/английский)
- Автоопределение языка браузера

### Размещение
Разместите свою версию где угодно — GitHub Pages, Vercel, Netlify, ваш сервер и т.д.

P.S. Особая благодарность https://github.com/sm1ky за предоставленное решение

