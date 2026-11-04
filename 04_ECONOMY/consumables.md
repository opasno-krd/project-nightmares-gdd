# Система Расходников: Искусство Баланса и Риска / Consumables System: Balance & Risk

## 🇷🇺 Русский

### Философия: Само-балансирующаяся экономика
Мы отказываемся от статичных цифр лечения. Эффективность зелий масштабируется от уровня персонажа. Дешевые зелья естественным образом устаревают, заставляя игрока инвестировать в более дорогие аналоги. Это создает стабильный, предсказуемый отток золота (Gold Sink).

### 1. Зелье Подмастерья (Apprentice Potion) — Стартовый выбор
Идеально для новичков, но быстро становится бесполезным.
*   **Мгновенный хил:** 10% от макс. HP.
*   **Доотхил (DoT):** 5 секунд. Формула одного тика (1 сек): `(30 - Уровень персонажа) / 2.5`.
*   **Эффект:** На 1-м уровне лечит ~68% HP (вау-эффект). На 30-м уровне лечит только 10% HP (сигнал к смене зелья).

### 2. Зелье Мастера (Master Potion) — Золотой стандарт
Надежное выживание для мид-гейма.
*   **Мгновенный хил:** 15% от макс. HP.
*   **Доотхил (DoT):** 3 секунды (3 тика). Формула одного тика: `(76 - Уровень персонажа) / 4`.
*   **Эффект:** На 1-м уровне лечит ~71% HP. На 65-м уровне лечит ~23% HP. Отличный экстренный хил, но не панацея.

### 3. Слеза Девы (Grand Healing) — Рейдовый эталон
Топовое зелье для сложных боссов и высокого уровня.
*   **Мгновенный хил:** 20% от макс. HP.
*   **Доотхил (DoT):** 2 секунды (2 тика). Формула одного тика: `(100 - Уровень персонажа) / 3`.
*   **Эффект:** На 1-м уровне лечит ~86% HP. На 65-м уровне лечит ~43% HP. Спасает жизнь в критических ситуациях на эндгейме.

### 4. Фляга Арлекина / Слёзы Мавроди (Harlequin's Flask) — Казино
Уникальное хай-лвл зелье. Это не просто лечение, это ставка на выживание и удачу, которая напрямую влияет на урон игрока.
*   **Мгновенный хил:** Рандом от 10% до 20%.
*   **Доотхил (DoT):** 1 секунда (2 тика по 0.5 сек). Очень быстрый burst-хил, так как на эндгейме нельзя стоять на месте.
*   **Формула одного тика:** `(Уровень персонажа / 4) * Множитель` (Множитель: рандом от 1.0 до 1.7).
*   **Вторичный эффект: Рулетка Урона (Damage Roulette):**
    *   При использовании зелье накладывает случайный модификатор к итоговому урону персонажа.
    *   *Диапазон:* От **-7%** до **+3%** (шаг 1%). Значение роллится один раз простым рандомом в этих пределах.
    *   *Тактика:* Танкам и хилерам этот модификатор не важен. Но для ДД (DPS) это критично. Игрок должен учитывать, что его урон временно просел или вырос, и адаптировать ротацию.
*   **UI и Нотификация:** При использовании на экране появляется четкая всплывающая подсказка: 
    *   *"Восстановлено [X]% HP. Модификатор урона: [Y]%"* (например, "+2% ATK" или "-5% ATK"). Цвет текста меняется: зеленый для плюса, красный для минуса.
*   **Эффект на 65-м уровне:** 
    *   *Плохой ролл:* ~42.5% HP и -7% к урону. Игрок выжил, но его DPS упал, что может привести к вайпу на таймере босса.
    *   *Хороший ролл:* ~75.2% HP и +3% к урону. Идеальный кайф, позволяющий агрессивно добить босса.
	
### 5. Правило Глубины Пояса
Все зелья стакаются до 20 000 единиц. В поясе (быстрый доступ) хранится максимум 2 единицы каждого типа. Когда первая выпивается, вторая мгновенно занимает её место.

---

## 🇬🇧 English

### Philosophy: Self-Balancing Economy
We reject static healing numbers. Potion effectiveness scales with the character's level. Cheap potions naturally become obsolete, forcing the player to invest in more expensive alternatives. This creates a stable, predictable Gold Sink.

### 1. Apprentice Potion — Starter Choice
Perfect for newbies, but quickly becomes useless.
*   **Instant Heal:** 10% of max HP.
*   **Heal over Time (DoT):** 5 seconds. Formula per tick (1 sec): `(30 - Character Level) / 2.5`.
*   **Effect:** At level 1, heals ~68% HP (wow effect). At level 30, heals only 10% HP (signal to upgrade).

### 2. Master Potion — The Gold Standard
Reliable survival for mid-game.
*   **Instant Heal:** 15% of max HP.
*   **Heal over Time (DoT):** 3 seconds (3 ticks). Formula per tick: `(76 - Character Level) / 4`.
*   **Effect:** At level 1, heals ~71% HP. At level 65, heals ~23% HP. Great emergency heal, but not a panacea.

### 3. Grand Healing (Virgin's Tear) — Raid Standard
Top-tier potion for difficult bosses and high levels.
*   **Instant Heal:** 20% of max HP.
*   **Heal over Time (DoT):** 2 seconds (2 ticks). Formula per tick: `(100 - Character Level) / 3`.
*   **Effect:** At level 1, heals ~86% HP. At level 65, heals ~43% HP. Saves lives in critical endgame situations.

### 4. Harlequin's Flask / Mavrodi's Tears — The Casino
A unique high-level potion. This is not just healing; it is a gamble on survival and luck that directly affects the player's damage output.
*   **Instant Heal:** Random from 10% to 20%.
*   **Heal over Time (DoT):** 1 second (2 ticks of 0.5 sec each). A very fast burst heal, as standing still in the endgame is impossible.
*   **Formula per tick:** `(Character Level / 4) * Multiplier` (Multiplier: random from 1.0 to 1.7).
*   **Secondary Effect: Damage Roulette:**
    *   Upon use, the potion applies a random modifier to the character's total damage output.
    *   *Range:* From **-7%** to **+3%** (1% step). The value is rolled once via simple random within these limits.
    *   *Tactics:* This modifier is irrelevant for Tanks and Healers. However, for DPS, it is critical. The player must account for their temporarily reduced or increased damage and adapt their rotation.
*   **UI & Notification:** Upon use, a clear pop-up appears on the screen: 
    *   *"Restored [X]% HP. Damage Modifier: [Y]%"* (e.g., "+2% ATK" or "-5% ATK"). Text color changes: green for a bonus, red for a penalty.
*   **Effect at Level 65:** 
    *   *Bad Roll:* ~42.5% HP and -7% damage. The player survived, but their DPS dropped, which could lead to a wipe on the boss timer.
    *   *Good Roll:* ~75.2% HP and +3% damage. Pure bliss, allowing the player to aggressively finish off the boss.
	
### 5. Belt Depth Rule
All potions stack up to 20,000 units. The belt (quick access) stores a maximum of 2 units of each type. When the first is consumed, the second instantly takes its place.