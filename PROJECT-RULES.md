# German Learning OS — Project Rules

## Core Principle
**Минимум действий пользователя → максимум автоматизации**

---

## Architecture Rules

### 1. One Object = One File
Каждый объект существует только один раз:
- Слово `haben` → `A0-Foundation/00-Vocabulary/haben.md`
- Грамматическое правило → `A0-Foundation/01-Grammar/sein-conjugation.md`
- Диалог → `A0-Foundation/03-Dialogue/dialogue1.md`

**Все уроки только ссылаются на эти файлы!**

### 2. No Duplicates
Если тема уже существует — она обновляется, не создаётся новый файл.

### 3. Course > Dictionary
Приоритет обновлений:
1. Lesson (урок)
2. Vocabulary (словарь)
3. Grammar (грамматика)
4. Exercises (упражнения)
5. Review (повторение)

### 4. Everything is Connected
- Каждое слово связано с уроками
- Каждая грамматика связана с уроками
- Каждая ошибка относится к модулю

---

## @GitHub Workflow

Пользователь пишет:
```
@GitHub
(материал, фото, текст, описание)
```

Система автоматически:
1. ✅ Анализирует материал
2. ✅ Определяет тему и модуль
3. ✅ Ищет существующие файлы
4. ✅ Обновляет Lesson
5. ✅ Обновляет Vocabulary
6. ✅ Обновляет Grammar
7. ✅ Обновляет Exercises
8. ✅ Обновляет Review
9. ✅ Обновляет связи
10. ✅ Коммитит в GitHub

---

## Module Structure

```
XX-Module-Name/
├── 00-Vocabulary/
│   ├── word1.md
│   ├── word2.md
│   └── vocabulary-index.md
├── 01-Grammar/
│   ├── rule1.md
│   ├── rule2.md
│   └── grammar-index.md
├── 02-Exercises/
│   ├── exercise1.md
│   └── exercises-index.md
├── 03-Dialogue/
│   ├── dialogue1.md
│   └── dialogue2.md
├── 04-Common-Mistakes/
│   └── mistakes-index.md
├── Lesson.md
├── Review.md
└── README.md
```

---

## Naming Conventions

- **Папки**: `XX-Module-Name` (числа для сортировки, kebab-case)
- **Файлы**: `lowercase-with-hyphens.md` или `word.md`
- **Commits**: `content:`, `update:`, `refactor:`, `system:` префиксы

---

## Priority

✅ iPhone-first (работает в Obsidian на мобиле)
✅ Минимум ручных действий
✅ Максимум автоматизации
✅ Чистая архитектура
✅ Масштабируемость на годы
