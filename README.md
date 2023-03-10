# goit-react-hw-01-components

Використовуй цей
[шаблон React-проекту](https://github.com/goitacademy/react-homework-template#readme)
як стартову точку своєї програми.

# Критерії приймання

- Створений репозиторій `goit-react-hw-01-components`.
- Компоненти всіх завдань рендеряться на одній сторінці, всередині спільного
  контейнера – кореневого компонента `<App>`.
- При здачі домашньої роботи є посилання на репозиторій з вихідним кодом
  проекту.
- В шапці репозиторія є посилання на живу сторінку на `GitHub pages`.
- Під час відвідування робочої сторінки (GitHub pages) завдання, в консолі
  відсутні помилки та попередження.
- Для кожного компонента є окрема папка з файлом React-компонента і файлом
  стилів.
- Для компонентів описані `propTypes`.
- Все, що компонент очікує у вигляді пропсів, передається йому під час виклику.
- Імена компонентів зрозумілі та описові.
- JS-код чистий і зрозумілий, використовується `Prettier`.
- Стилізація виконана `CSS-модулями` або `Styled Components`, тому класи в
  результуючому DOM відрізнятимуться від прикладів.
- Достатньо базової стилізації застосунку, насамперед він повинен працювати, а
  вже потім бути гарним. Приділяй 20% часу на CSS і 80% на JS.

## Завдання

# Профіль соціальної мережі

Необхідно створити компонент `<Profile>`, за допомогою якого ми могли б відображати інформацію про користувача соціальної мережі. Дані про користувача лежать у файлі [user.json](./user.json).

![Прев'ю компонента Profile align="center"](https://github.com/goitacademy/react-homework/blob/master/homework-01/social-profile/preview.png)

## Опис компонента `<Profile>`

Компонент повинен приймати кілька пропсів з інформацією про користувача:

- `username` — ім'я користувача
- `tag` — тег в соціальній мережі без `@`
- `location` — місто і країна
- `avatar` — посилання на зображення
- `stats` — об'єкт з інформацією про активності

Компонент повинен створювати DOM елемент наступної структури.

```html
<div class="profile">
  <div class="description">
    <img
      src="https://cdn-icons-png.flaticon.com/512/1077/1077012.png"
      alt="User avatar"
      class="avatar"
    />
    <p class="name">Petra Marica</p>
    <p class="tag">@pmarica</p>
    <p class="location">Salvador, Brasil</p>
  </div>

  <ul class="stats">
    <li>
      <span class="label">Followers</span>
      <span class="quantity">1000</span>
    </li>
    <li>
      <span class="label">Views</span>
      <span class="quantity">2000</span>
    </li>
    <li>
      <span class="label">Likes</span>
      <span class="quantity">3000</span>
    </li>
  </ul>
</div>
```

## Приклад використання

```js
import user from 'путь/к/user.json;

<Profile
  username={user.username}
  tag={user.tag}
  location={user.location}
  avatar={user.avatar}
  stats={user.stats}
/>
```

