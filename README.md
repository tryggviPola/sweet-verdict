# Sweet Verdict

A pocket lookup tool that tells you whether a sweetener or sugar substitute is a good choice for **pre-diabetes and weight loss**.

Type an ingredient from a "sugar-free" label, in English, in Russian or as an E-number (`maltitol`, `мальтит`, `E965`), and get a color-coded rating with a plain-language explanation of the downsides.

*Русская версия — внизу.*

## Features

- 38 sweeteners, sugars and sugar-like ingredients
- Four ratings: **Good**, **Ok**, **Caution**, **Avoid**
- Glycemic index (GI) and downsides for each entry
- Search by English name, Russian name, alternative names or E-number
- Filter by rating
- English and Russian interface (switch with the RU/EN button)
- Light and dark mode, follows your phone's setting
- Installs on an iPhone home screen like a normal app

## What the ratings mean

| Rating | Meaning |
|---|---|
| **Good** | Does not raise blood sugar. Few known downsides. |
| **Ok** | Does not raise blood sugar, but has a catch (limited evidence, side effects, or possible health concerns). |
| **Caution** | Small effect on blood sugar and/or likely digestive side effects. Use sparingly. |
| **Avoid** | Raises blood sugar, or is harmful in other ways (for example, fructose and the liver). |

**GI (glycemic index)** shows how fast a food raises blood sugar. Pure glucose is 100 and table sugar is about 65.

## Files

| File | What it is |
|---|---|
| `index.html` | The entire app (code and data in one file) |
| `icon.png` | The home-screen icon |

There is nothing to install or build. Both files must stay in the same folder.

## Publish it with GitHub Pages

1. Create a public repository on GitHub.
2. Upload `index.html`, `icon.png` and this `README.md`.
3. Go to **Settings → Pages**, choose the `main` branch and save.
4. After a minute or two the app is live at `https://YOUR-USERNAME.github.io/YOUR-REPO/`.

## Add it to an iPhone

1. Open the link in **Safari** (not Chrome).
2. Tap **Share → Add to Home Screen**.

If you update the icon later, delete the old home-screen icon and add the app again. The iPhone keeps the old icon until you do.

## Add or edit an ingredient

All entries are in the `D` list near the bottom of `index.html`. Each one looks like this:

```js
{n:["Stevia","Стевия"],          // names: [English, Russian]
 a:"E960 steviol glycosides",    // other names to search by
 c:"g",                          // rating: g = Good, o = Ok, c = Caution, a = Avoid
 gi:"0",                         // glycemic index (text)
 t:["English explanation.","Объяснение по-русски."]}
```

Separate entries with a comma. The list is sorted by rating automatically.

## Limitations

- Needs an internet connection (no offline mode yet).
- Does not scan labels or read a whole ingredient list yet.
- GI values are approximate and vary by source.

## Disclaimer

This is general information, **not medical advice**. The ratings are one person's judgment for one specific situation (pre-diabetes and weight loss), not an official standard. Talk to your doctor or dietitian about your own case. "Sugar-free" only means no table sugar, so always read the full ingredient list.

---

# Sweet Verdict (по-русски)

Карманный справочник, который подсказывает, подходит ли подсластитель или заменитель сахара при **преддиабете и снижении веса**.

Введите название ингредиента с этикетки «без сахара» по-английски, по-русски или E-номер (`maltitol`, `мальтит`, `E965`) и получите цветную оценку с понятным объяснением вреда.

## Возможности

- 38 подсластителей, сахаров и похожих ингредиентов
- Четыре оценки: **Хорошо**, **Нормально**, **Осторожно**, **Избегать**
- Гликемический индекс (ГИ) и недостатки каждого ингредиента
- Поиск по английскому и русскому названию, другим названиям и E-номеру
- Фильтр по оценке
- Интерфейс на английском и русском (кнопка RU/EN)
- Светлая и тёмная тема
- Устанавливается на экран iPhone как обычное приложение

## Как установить на iPhone

1. Откройте ссылку в **Safari** (не в Chrome).
2. Нажмите **Поделиться → На экран «Домой»**.

## Важно

Это общая информация, **а не медицинский совет**. Оценки — это суждение для одной конкретной ситуации (преддиабет и снижение веса), а не официальный стандарт. Свой случай обсудите с врачом или диетологом. «Без сахара» значит лишь «без столового сахара», поэтому всегда читайте полный состав.
