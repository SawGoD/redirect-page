# ➡️ Страница перенаправления

Простая страница перенаправления, которая позволяет перенаправлять пользователей на другие URL-адреса с задержкой.

### 🧠 Что это такое?

Telegram Desktop на Windows некорректно открывает **внешние глубокие ссылки** (такие как `v2box://`, `happ://`, `clash://...` и т.д.), когда они приходят из браузера или сообщения.

## Использование

Добавьте параметр `redirect_to` к URL страницы:

```
https://sawgod.github.io/redirect-page/?redirect_to=clash://install-config?url=SUB_URL
```

### 🤖 Автоматический выбор темы по ОС

Используйте параметр `system` для автоматического определения темы на основе операционной системы пользователя:

```
https://sawgod.github.io/redirect-page/?system&redirect_to=YOUR_URL
```

**Маппинг ОС → Темы:**
- 🪟 **Windows** → `microsoft` (Microsoft Fluent Design)
- 🍎 **macOS / iOS** → `apple` (Apple стиль)
- 🤖 **Android** → `google` (Material Design)
- 🐧 **Linux / другие** → `telegram` (стандартная тема)

### 🎨 Ручной выбор темы

Вы можете выбрать конкретную тему оформления с помощью параметра `theme`:

```
https://sawgod.github.io/redirect-page/?theme=THEME_NAME&redirect_to=YOUR_URL
```

**Доступные темы:**
- `telegram` - Стандартная тема (используется по умолчанию)
- `retro` - Ретро-стиль с анимациями
- `pixel` - Пиксельная игровая тема в стиле 8-bit
- `smart` - Современная тема с синим дизайном и анимациями
- `glass` - Стеклянная тема с холодным градиентом, вдохновлённая glassmorphism
- `neon` - Неоновая тема с изящным градиентом
- `aurora` - Северное сияние с мягкими анимациями
- `soft` - Мягкая розово-фиолетовая тема с карточками
- `mono` - Ч/б дизайн с крупными цифрами и строгой типографикой
- `simple` - Простая монохромная тема
- `minimal` - Минималистичная тема
- `apple` - Стиль Apple
- `google` - Стиль Google Material Design
- `microsoft` - Стиль Microsoft Fluent Design

**Примеры:**

```
# Стандартная тема (Telegram) - тему указывать не нужно
https://sawgod.github.io/redirect-page/?redirect_to=YOUR_URL

# Автоопределение темы по ОС (рекомендуется)
https://sawgod.github.io/redirect-page/?system&redirect_to=YOUR_URL

# Тема Microsoft (ручной выбор)
https://sawgod.github.io/redirect-page/?theme=microsoft&redirect_to=YOUR_URL

# Ретро тема
https://sawgod.github.io/redirect-page/?theme=retro&redirect_to=YOUR_URL

# Современная тема Smart
https://sawgod.github.io/redirect-page/?theme=smart&redirect_to=YOUR_URL
```

> **Примечание:** Параметр `?theme` имеет приоритет над `?system`. Если указаны оба, будет использована тема из `?theme`.

## Особенности

- 🤖 **Автоопределение темы по ОС** - система автоматически выбирает подходящую тему
- ⏱️ Автоматическое перенаправление через 7 секунд
- 🔄 Кнопка для немедленного перенаправления
- 📱 Адаптивный дизайн (мобильные устройства и десктоп)
- 🌐 Автоматическое определение языка (русский/английский)
- 🌙 Поддержка темной темы (light/dark mode)
- 🎨 Множество тем оформления на выбор
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
  <summary>Pixel (8-bit игровая тема)</summary>

  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/pixel_light.png)  |  ![](img/pixel_dark.png)
</details>

<details>
  <summary>Smart</summary>

  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/smart_light.png)  |  ![](img/smart_dark.png)
</details>

<details>
  <summary>Glass</summary>

  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/glass_light.png)  |  ![](img/glass_dark.png)
</details>

<details>
  <summary>Neon</summary>

  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/neon_light.png)  |  ![](img/neon_dark.png)
</details>

<details>
  <summary>Soft</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/preview_light.png)  |  ![](img/preview_dark.png)
</details>

<details>
  <summary>Aurora</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/aurora_light.png)  |  ![](img/aurora_dark.png)
</details>

<details>
  <summary>Mono</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/mono_light.png)  |  ![](img/mono_dark.png)
</details>

<details>
  <summary>Simple</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/simple_light.png)  |  ![](img/simple_dark.png)
</details>

<details>
  <summary>Minimal</summary>
  
  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/minimal_light.png)  |  ![](img/minimal_dark.png)
</details>

<details>
  <summary>System (Apple, Google, Microsoft)</summary>

  Светлая тема             |  Темная тема
:-------------------------:|:-------------------------:
![](img/apple_light.png)  |  ![](img/apple_dark.png)
![](img/google_light.png)  |  ![](img/google_dark.png)
![](img/microsoft_light.png)  |  ![](img/microsoft_dark.png)
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

