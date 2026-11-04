# Дальний бой и Система Колчана / Ranged Combat & Quiver System

## 🇷🇺 Русский

### Философия: Тактическая адаптация без физики
Мы отказываемся от сложной баллистики и упреждения. Дальний бой — это мгновенный отклик, управление дистанцией и адаптация под тип брони врага.

### 1. Инвентарь и HUD (Колчан)
Стрелы — это расходник, но они не должны захламлять инвентарь.
*   **Слот в инвентаре:** Специальный слот "Колчан". Стрелы стакаются до **20 000 единиц** в одной ячейке.
*   **Нижний HUD:** Отдельный, всегда видимый слот колчана. Отображает иконку текущих стрел и их точное количество (например, "14,500").
*   **Кнопка переключения:** Рядом со слотом в HUD находится кнопка смены режима стрельбы (или привязка на клавишу `R` / колесико мыши).

### 2. Режимы Стрельбы (Адаптивный Колчан)
Игрок мгновенно переключается между двумя режимами, не залезая в инвентарь:
*   **Режим "Яблочко" (Прямой выстрел):** 
    *   *Траектория:* Плоская, высокая скорость полета.
    *   *Применение:* Максимальная дальность, мобильные цели, легкая броня. Стандартный режим.
*   **Режим "Навесом" (Навесная траектория):**
    *   *Траектория:* Высокая дуга, меньшая дальность, стрела летит чуть дольше.
    *   *Применение:* Позволяет стрелять через низкие укрытия. Наносит **повышенный урон по тяжелой броне** на близкой и средней дистанции за счет кинетической энергии падения.

### 3. Прогрессия и Крафт (Книга "Меткая стрельба")
Лучник не начинает игру с возможностью крафта. Это навык, который нужно заслужить.
*   **Разблокировка:** На **15-м уровне** прокачки книги *"Меткая стрельба"* (Marksmanship) игрок получает пассивное знание "Основы лучника".
*   **Крафт:** Это знание открывает рецепт создания стрел у кузнеца или на верстаке. Игрок комбинирует материалы (дерево, металл для наконечников, перья) для создания физических стрел. Это и есть синергия пассивок книги и активного действия.

### 4. Активный навык: Магические стрелы (Magic Arrows)
Чтобы лучник не чувствовал себя беспомощным, если он забыл купить стрелы или застрял в глубоком данже, книга дает аварийный навык.
*   **Механика:** Создает эфирные стрелы, которые заполняют колчан.
*   **Лимит:** Максимум **500 штук**. Они не заменяют физические стрелы (у них средний урон и пробитие).
*   **Откат (Cooldown):** Восстановление до максимума занимает **3 минуты**.
*   **Тактика:** Это страховка ("казино" на выживание), а не основа билда. Игрок всегда будет стремиться использовать крафтовые физические стрелы для максимального DPS.

---

## 🇬🇧 English

### Philosophy: Tactical Adaptation Without Physics
We reject complex ballistics and leading targets. Ranged combat is about instant feedback, distance management, and adapting to enemy armor types.

### 1. Inventory & HUD (The Quiver)
Arrows are consumables, but they shouldn't clutter the inventory.
*   **Inventory Slot:** A dedicated "Quiver" slot. Arrows stack up to **20,000 units** in a single cell.
*   **Bottom HUD:** A dedicated, always-visible quiver slot. It displays the current arrow icon and exact count (e.g., "14,500").
*   **Toggle Button:** Next to the slot in the HUD is a button to switch firing modes (or bound to `R` key / mouse wheel).

### 2. Firing Modes (Adaptive Quiver)
The player instantly switches between two modes without opening the inventory:
*   **"Bullseye" Mode (Direct Fire):** 
    *   *Trajectory:* Flat, high projectile speed.
    *   *Use Case:* Maximum range, mobile targets, light armor. The default mode.
*   **"Arcing" Mode (Plunging Fire):**
    *   *Trajectory:* High arc, shorter range, slightly longer flight time.
    *   *Use Case:* Allows shooting over low cover. Deals **bonus damage to heavy armor** at close and medium range due to the kinetic energy of the falling arrow.

### 3. Progression & Crafting ("Marksmanship" Book)
An archer doesn't start with crafting capabilities. It's a skill that must be earned.
*   **Unlock:** At **Level 15** of the *"Marksmanship"* skill book, the player gains the passive knowledge "Archery Basics".
*   **Crafting:** This knowledge unlocks the arrow crafting recipe at the blacksmith or workbench. The player combines materials (wood, metal tips, feathers) to craft physical arrows. This is the synergy of the book's passives and active gameplay.

### 4. Active Skill: Magic Arrows
To ensure the archer isn't helpless if they forget to buy arrows or get stuck in a deep dungeon, the book provides an emergency skill.
*   **Mechanic:** Creates ethereal arrows that fill the quiver.
*   **Limit:** Maximum **500 units**. They do not replace physical arrows (they have average damage and penetration).
*   **Cooldown:** Regenerating to the maximum cap takes **3 minutes**.
*   **Tactics:** This is a safety net ("survival casino"), not the core of the build. The player will always strive to use crafted physical arrows for maximum DPS.