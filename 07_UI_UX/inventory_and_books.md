# Инвентарь и Меню Книг Навыков / Inventory & Skill Books Menu

## 🇷🇺 Русский

### Философия: Сетка и Анатомия
Инвентарь — это классическая, понятная сетка в стиле Diablo. Меню книг навыков использует анатомический интерфейс для атмосферы, но механически опирается только на уровневые ограничения, чтобы избежать сложностей с балансировкой.

### 1. Инвентарь (Правая треть экрана)
При открытии (клавиша `I`) инвентарь занимает правую 1/3 экрана. Слева от него открывается панель экипировки и книг. Инвентарь — это плавающее окно, которое **НЕ перекрывает** нижний HUD.

**Сетка инвентаря:**
- **Размер:** 6x12 ячеек (72 слота).
- **Размеры предметов (в ячейках):**
  - Зелья, кольца, амулеты: 1x1 (1 ячейка)
  - Пояс: 2x1 (2 ячейки)
  - Перчатки, сапоги, шлем, книги навыков: 2x2 (4 ячейки)
  - Одноручное оружие: 1x3 (3 ячейки)
  - Броня (нагрудник), Двуручное оружие: 2x3 (6 ячеек)

**Слоты экипировки (Классика):**
Шлем, Амулет, Нагрудник, Левая рука, Правая рука, 2 Кольца, Пояс, Сапоги. Никакого разделения на «верх» и «низ» — только цельный нагрудник.

### 2. Меню Книг Навыков (Анатомический интерфейс и Туман Войны)
Это выезжающий модуль слева от инвентаря. Игрок видит **силуэт своего персонажа**. Книги навыков «вкладываются» в части тела, создавая визуальную связь. Ограничением для размещения книги является **только уровень слота и уровень самой книги**.

**UI Книги (Туман Войны / Fog of War):**
Когда игрок кликает на экипированную книгу, она открывается в интерфейсе ровно на той странице, до которой он её прокачал.
*   **Текущая страница:** Показывает текущие пассивные бонусы (например, "+5% к скорости бега").
*   **Следующий навык:** Иконка следующего активного навыка **скрыта (размыта или закрыта чернильным пятном)**. Игрок видит только индикатор прогресса: *"Вложите еще 3 SP, чтобы открыть страницу"*.
*   **Разблокировка:** Как только игрок вливает нужное количество SP, страница с анимацией переворачивается. Открывается иконка активного навыка, которую можно **перетащить на панель быстрого доступа**.
*   **Будущее:** Что находится на следующих страницах — игрок не видит. Это стимулирует исследование, обмен опытом и создание гайдов сообществом (YouTube, форумы).

**Прогрессия слотов (Всего 7 слотов):**
1. **Старт (3 слота):** *Левая рука, Правая рука, Грудь*
2. **Уровень 30 (Открываются 4-й и 5-й слоты):** *Ноги*
3. **Уровень 45 (Открывается 6-й слот):** *Живот/Кор*
4. **Максимальный уровень (Открывается 7-й слот):** *Голова*

### 3. Таймеры и Визуализация (7 дней и Кровотечение)
- **Таймер 7 дней:** В углу иконки предмета в инвентаре появляется тонкая цветная полоска. Зеленая (свежий дроп) -> Желтая (прошло 4 дня) -> Красная (осталось <24 часов).
- **Замороженное кровотечение:** Когда игрок накладывает повязку (F), рядом со столбом HP появляется иконка бинта с обратным отсчетом (15 сек). Если игрок делает кувырок, иконка «рвется» с характерным звуком, и таймер исчезает.

---

## 🇬🇧 English

### Philosophy: Grid and Anatomy
The inventory is a classic, intuitive Diablo-style grid. The Skill Books menu uses an anatomical interface for atmosphere, but mechanically relies only on level restrictions to avoid balancing complexities.

### 1. Inventory (Right 1/3 of the screen)
When opened (`I` key), the inventory takes up the right 1/3 of the screen. To its left, the equipment and books panel slides out. The inventory is a floating window that does **NOT overlap** the bottom HUD.

**Inventory Grid:**
- **Size:** 6x12 cells (72 slots).
- **Item Sizes (in cells):**
  - Potions, rings, amulets: 1x1 (1 cell)
  - Belt: 2x1 (2 cells)
  - Gloves, boots, helmet, skill books: 2x2 (4 cells)
  - One-handed weapons: 1x3 (3 cells)
  - Armor (Chest), Two-handed weapons: 2x3 (6 cells)

**Equipment Slots (Classic):**
Helmet, Amulet, Chest, Left Hand, Right Hand, 2 Rings, Belt, Boots. No "top/bottom" armor split — just a unified chest piece.

### 2. Skill Books Menu (Anatomical Interface & Fog of War)
This is a sliding module to the left of the inventory. The player sees a **silhouette of their character**. Skill books are "slotted" into body parts, creating a visual connection. The only restriction for placing a book is the **slot level and the book's level**.

**Book UI (Fog of War):**
When the player clicks on an equipped book, it opens in the interface exactly on the page they have leveled up to.
*   **Current Page:** Shows current passive bonuses (e.g., "+5% run speed").
*   **Next Skill:** The icon of the next active skill is **hidden (blurred or covered in an ink blot)**. The player only sees a progress indicator: *"Invest 3 more SP to turn the page"*.
*   **Unlock:** Once the player invests the required SP, the page turns with an animation. The active skill icon is revealed and can be **dragged to the hotbar**.
*   **The Future:** What lies on the next pages is unseen. This encourages exploration, knowledge sharing, and community-driven content (YouTube guides, wikis).

**Slot Progression (Total 7 Slots):**
1. **Start (3 slots):** *Left Hand, Right Hand, Chest*
2. **Level 30 (Unlocks 4th and 5th slots):** *Legs*
3. **Level 45 (Unlocks 6th slot):** *Stomach/Core*
4. **Max Level (Unlocks 7th slot):** *Head*

### 3. Timers & Visualization (7 Days & Bleeding)
- **7-Day Timer:** A thin colored bar appears in the corner of the item icon. Green (fresh drop) -> Yellow (4 days passed) -> Red (<24 hours left).
- **Suppressed Bleeding:** When the player bandages (F), a bandage icon with a countdown (15 sec) appears next to the HP bar. If the player dodge rolls, the icon "rips" with a distinct sound, and the timer disappears.