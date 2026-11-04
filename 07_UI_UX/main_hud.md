# Главный HUD игрока / Main Player HUD

## 🇷🇺 Русский

### Философия дизайна
Мы не изобретаем велосипед. Мы берем проверенные временем решения (Diablo-подобный пояс и плавающий инвентарь) и подкручиваем их под нашу механику. Главный принцип: **минимум визуального шума, максимум информации**. Инвентарь — это плавающее окно справа, которое **НЕ перекрывает** нижний HUD, оставляя его всегда видимым.

### Структура нижнего модуля
Главный интерфейс — это горизонтальная панель внизу экрана, разделенная на три зоны:

#### 1. Левая зона: Мана и Дебаффы
- **Столб MP (Mana Points):** Вертикальная полоса слева. Синий цвет, заполняется снизу вверх.
- **Слоты дебаффов:** Расположены рядом со столбом MP. Это не выделенные "ячейки", а **появляющиеся иконки**. Когда на игроке висит эффект (кровотечение, яд, шок), рядом с MP появляется красочная иконка с таймером. Когда эффект спадает — иконка исчезает. Это снижает визуальный шум в спокойные моменты.

#### 2. Центральная зона: Пояс расходников
- **Расположение:** Между столбами HP и MP.
- **Слоты:** 4 слота под расходники (базовый модульный пояс, доступен с 1 уровня):
  - **Слот 1:** Зелье HP (красная иконка)
  - **Слот 2:** Зелье MP (синяя иконка)
  - **Слот 3:** Бинты (белая/серая иконка)
  - **Слот 4:** Бафф-зелье (зеленая/фиолетовая иконка, детали в будущем)
- **Глубина пояса:** 2 позиции. То есть в каждом слоте хранится 2 единицы расходника на быстром доступе. Когда первая используется, вторая автоматически занимает её место.
- **Управление:** Клавиши 1-4 или клик мышью.

#### 3. Правая зона: Здоровье и Опыт
- **Столб HP (Health Points):** Вертикальная полоса справа. Красный цвет, заполняется снизу вверх. Расположение справа — осознанный выбор: так как инвентарь находится справа и не перекрывает HUD, глаз игрока всегда видит свой HP, даже когда он управляет экипировкой.
- **Шкала опыта:** Расположена под поясом, по центру. Разбита на **5% отсечки** (визуальные метки каждые 5%). Это дает игроку четкое понимание прогресса без необходимости смотреть в меню.

### Что мы НАМЕРЕННО не показываем
- **Стамина:** Она есть в механике (кувырки, навыки), но не показывается как отдельный столб. Почему? Потому что игроки всё равно бегают, и искусственное ограничение выносливости только бесит. Стамина восстанавливается автоматически, и игрок чувствует её через геймплей (нельзя спамить кувырками), а не через цифру на экране.

---

## 🇬🇧 English

### Design Philosophy
We don't reinvent the wheel. We take time-tested solutions (Diablo-like belt and floating inventory) and tweak them for our mechanics. Main principle: **minimum visual noise, maximum information**. The inventory is a floating window on the right that does **NOT overlap** the bottom HUD, keeping it always visible.

### Bottom Module Structure
The main interface is a horizontal panel at the bottom of the screen, divided into three zones:

#### 1. Left Zone: Mana & Debuffs
- **MP Bar (Mana Points):** Vertical bar on the left. Blue color, fills from bottom to top.
- **Debuff Slots:** Located next to the MP bar. These are not fixed "cells", but **appearing icons**. When the player has an effect (bleeding, poison, shock), a colorful icon with a timer appears next to MP. When the effect fades — the icon disappears. This reduces visual noise in calm moments.

#### 2. Center Zone: Consumable Belt
- **Location:** Between HP and MP bars.
- **Slots:** 4 slots for consumables (basic modular belt, available from level 1):
  - **Slot 1:** HP Potion (red icon)
  - **Slot 2:** MP Potion (blue icon)
  - **Slot 3:** Bandages (white/gray icon)
  - **Slot 4:** Buff Potion (green/purple icon, details in future)
- **Belt Depth:** 2 positions. Each slot stores 2 consumable units on quick access. When the first is used, the second automatically takes its place.
- **Controls:** Keys 1-4 or mouse click.

#### 3. Right Zone: Health & Experience
- **HP Bar (Health Points):** Vertical bar on the right. Red color, fills from bottom to top. Placement on the right is a conscious choice: since the inventory is on the right and doesn't overlap the HUD, the player's eye always sees their HP, even when managing equipment.
- **Experience Bar:** Located below the belt, in the center. Divided into **5% segments** (visual markers every 5%). This gives the player clear progress understanding without opening menus.

### What we INTENTIONALLY don't show
- **Stamina:** It exists in mechanics (dodge rolls, skills), but is not shown as a separate bar. Why? Because players run anyway, and artificial stamina limits only frustrate. Stamina regenerates automatically, and the player feels it through gameplay (can't spam dodges), not through a number on screen.