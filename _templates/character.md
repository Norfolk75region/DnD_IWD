---
datetime: <% tp.date.now("YYYY-MM-DDTHH:mm") %>
tags:
  - 🎭
aliases:
  - <%*
let title = tp.file.title;
// Находим индекс первого буквенно-цифрового символа
let firstValidCharIndex = title.search(/[a-zA-Zа-яА-Я0-9]/);
if (firstValidCharIndex === -1) {
  // Если в строке вообще нет букв/цифр, оставляем как есть (или можно вернуть пустую строку)
  trimmedTitle = title;
} else {
  // Обрезаем всё до первого валидного символа
  trimmedTitle = title.slice(firstValidCharIndex);
}
-%>
<%- trimmedTitle %>
Имя:
Игрок: NPC
Раса:
Класс:
Пол:
Уровень:
Возраст:
Рост:
Вес:
---
# <% tp.file.title%>
