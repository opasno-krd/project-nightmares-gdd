# Матрица Урона, Статусы и Алхимия / Damage Matrix, Status Effects & Alchemy

## 🇷🇺 Русский

### Философия: Физическая логика и Тактическая Глубина
Матрица урона построена на здравом смысле. Нет абстрактных цифр, есть логика взаимодействия материалов. DoT-эффекты и алхимия жестко привязаны к типу оружия и броне, превращая бой в тактические шахматы.

### 1. Классы Брони и Физический Урон
*   **Тяжелая / Ультратяжелая (Паладины, Танки, Рыцари):** 
    *   *Рубящий (Slashing):* Отличная защита (0.5x). Меч соскальзывает или застревает.
    *   *Дробящий (Blunt):* Хорошая защита от легкого дробления, но тяжелые молоты вызывают **потерю выносливости** и оглушение, даже если HP не падает сильно.
    *   *Колющий (Piercing):* **Слабая защита** (1.3x). Арбалетный болт или стилет в щель сочленения проходит насквозь, игнорируя часть брони.
*   **Легкая / Средняя (Ловкачи, Барды, Плуты, Охотники):**
    *   *Защита:* Сбалансированная (1.0x) против Рубящего, Дробящего и Колющего. Главный бонус — высокая подвижность для уклонения.
*   **Робы (Маги, Жрецы, Клерик):**
    *   *Защита:* Нулевая физическая защита (1.5x ко всем физическим типам). Выживание зависит от дистанции и контроля.

### 2. Элементальная Матрица (Стихии vs Броня)
*   **Электричество (Lightning):** *Тяжелая:* **Отлично** (1.5x, клетка Фарадея + стан). *Легкая:* Плохо (0.8x). *Робы:* **Почти 0** (0.5x, диэлектрик).
*   **Холод / Лёд (Cold):** *Тяжелая:* Хорошо (1.2x, хрупкость металла). *Легкая:* Отлично (1.4x). *Робы:* **Вымораживает наглухо** (1.8x, мгновенное промерзание и замедление каста).
*   **Огонь (Fire):** *Тяжелая:* Почти не повреждает (0.6x). *Легкая:* Умеренно (1.1x). *Робы:* **Бонусный урон** (1.5x, мгновенное возгорание, кроме огнеупорных зачарований).
*   **Земля (Earth):** Считается **Дробящим (Blunt)** уроном с элементами замедления.
*   **Чистая Магия / Аркана (Arcane):** Игнорирует физическую броню на 100%. Урон идет по "Магическому Сопротивлению". **Правило:** В игре нет школы магии ядов. Яд — только физическая алхимия.

### 3. Статусные Эффекты (DoT) и Привязка к Типу Урона
DoT не существуют в вакууме. Их сила зависит от типа оружия, нанесшего урон.

*   **Кровотечение (Bleeding):**
    *   *От Колющего (Piercing):* **Слабое.** Глубокая, узкая рана. Кровь быстро сворачивается. Минимальный DoT.
    *   *От Рубящего (Slashing):* **Сильное.** Широкий разрез. Кровь хлещет, мощный DoT.
    *   *Взаимодействие с броней:* В **тяжелой броне** — это ад (внутренние разрывы). Наложить повязку (F) почти невозможно. Лечится *только* зельями (йод/зеленка). В **легкой броне** и **робах** (ткань как тампон) повязки работают отлично.
*   **Яд (Poison):**
    *   *От Колющего (Piercing):* **Идеальное проникновение.** Яд вводится в кровоток, игнорируя броню. Отравленная рапира — имба против танков.
    *   *От Рубящего/Дробящего (Slashing/Blunt):* **Поверхностное.** Яд остается на поверхности. Бесполезен против тяжелых лат (просто вытирается). Эффективен против легкой брони и роб.

### 4. Алхимия, Яды и Контроль Зоны (Area Denial)
Яд — это грязная работа плутов и алхимиков, требующая тактического применения.

*   **Метамая Склянка (AoE Газ):**
    *   *Анти-Хил Зона:* Пока персонаж в облаке, **естественная регенерация и лечение зельями полностью блокируются**. Токсин нейтрализует хил.
    *   *Респираторный дистресс:* Вдох газа вызывает кашель (стан/замедление, прерывает касты).
    *   *Эффект "Внутренний дискомфорт" (Тяжелая броня):* Газ попадает внутрь герметичных лат и не выветривается. -50% к регену выносливости, 10% шанс кашля при получении физ. урона.
    *   *Контрплей (Сопротивление Яду):* Высокий резист (от книг, бижутерии, еды) позволяет игнорировать блокировку хила и спокойно лечиться прямо в облаке.
*   **Нанесение на Оружие (Weapon Coating):**
    *   Дает **10-15 попаданий** (или длится 2 минуты). Урон = Физ. урон + DoT яда. Подчиняется правилам Матрицы (Колющий = внутрь, Рубящий = снаружи).
*   **Отравление Колчана (Poisoned Quiver):**
    *   Лучник окунает наконечники. Вся партия стрел (до 500 шт) получает яд. Урон яда чуть ниже, чем с клинка (баланс дистанции), но идеально для режима "Навесом".
*   **Типы Ядов:**
    *   *Накопительные (Stacking):* (Напр. Белладонна). Каждое попадание усиливает DoT или продлевает время (до капа в 3 стека). Для долгих боев с боссами.
    *   *Острые (Acute):* (Напр. Сыворотка Гадюки). Мгновенный мощный урон при первом попадании. Повторное нанесение не стакается, а лишь **освежает таймер**. Для burst-урона и PvP.

---

## 🇬🇧 English

### Philosophy: Physical Logic & Tactical Depth
The damage matrix is built on common sense. No abstract numbers, just material interaction logic. DoTs and alchemy are strictly tied to weapon and armor types, turning combat into tactical chess.

### 1. Armor Classes & Physical Damage
*   **Heavy / Ultra-Heavy (Paladins, Tanks, Knights):** 
    *   *Slashing:* Excellent defense (0.5x). Swords glance off or get stuck.
    *   *Blunt:* Good defense against light blunt, but heavy hammers cause **Stamina Drain** and stagger.
    *   *Piercing:* **Weak defense** (1.3x). Crossbow bolts or stilettos punch through joint gaps, ignoring armor.
*   **Light / Medium (Agility, Bards, Rogues, Hunters):**
    *   *Defense:* Balanced (1.0x) against Slashing, Blunt, and Piercing. Main bonus is high mobility to dodge.
*   **Robes (Mages, Priests, Clerics):**
    *   *Defense:* Zero physical defense (1.5x to all physical types). Survival depends on distance and crowd control.

### 2. Elemental Matrix (Elements vs Armor)
*   **Lightning:** *Heavy:* **Excellent** (1.5x, Faraday cage + stun). *Light:* Poor (0.8x). *Robes:* **Almost 0** (0.5x, dielectric).
*   **Cold / Ice:** *Heavy:* Good (1.2x, brittle metal). *Light:* Excellent (1.4x). *Robes:* **Freezes Solid** (1.8x, instant freezing and cast slow).
*   **Fire:** *Heavy:* Almost no damage (0.6x). *Light:* Moderate (1.1x). *Robes:* **Bonus Damage** (1.5x, instant ignition, except fireproof enchantments).
*   **Earth:** Treated as **Blunt** damage with a slow effect.
*   **Arcane / Pure Magic:** Ignores physical armor 100%. Damage goes against "Magic Resistance". **Rule:** No School of Poison Magic exists. Poison is strictly physical alchemy.

### 3. Status Effects (DoTs) & Damage Type Dependency
DoTs do not exist in a vacuum. Their strength depends on the weapon type that inflicted the damage.

*   **Bleeding:**
    *   *From Piercing:* **Weak.** Deep, narrow wound. Blood clots fast. Minimal DoT.
    *   *From Slashing:* **Strong.** Wide gash. Blood pours, heavy DoT.
    *   *Armor Interaction:* In **Heavy Armor**, bleeding is hell (internal ruptures). Bandaging (F) is nearly impossible. Cured *only* by potions (iodine). In **Light Armor** and **Robes** (fabric acts as tampon), bandages work perfectly.
*   **Poison:**
    *   *From Piercing:* **Perfect Penetration.** Poison is injected into the bloodstream, ignoring armor. A poisoned rapier is imba against tanks.
    *   *From Slashing/Blunt:* **Surface Poisoning.** Poison stays on the surface. Useless against heavy plate (just wipes off). Effective against light armor and robes.

### 4. Alchemy, Poisons & Area Denial
Poison is dirty work for rogues and alchemists, requiring tactical application.

*   **Throwable Vial (AoE Gas):**
    *   *Anti-Heal Zone:* While inside the cloud, **natural regen and potion healing are completely blocked**. Toxin neutralizes heals.
    *   *Respiratory Distress:* Inhaling gas causes coughing (stun/slow, interrupts casts).
    *   *Heavy Armor "Chafing" Debuff:* Gas gets trapped inside airtight plate. -50% stamina regen, 10% chance to cough on physical hit.
    *   *Counterplay (Poison Resistance):* High resistance (from books, jewelry, food) allows ignoring the heal block and healing safely inside the cloud.
*   **Weapon Coating:**
    *   Provides **10-15 hits** (or lasts 2 mins). Damage = Phys. damage + Poison DoT. Follows Matrix rules (Piercing = internal, Slashing = surface).
*   **Poisoned Quiver:**
    *   Archer dips arrowheads. The whole batch (up to 500) gets poisoned. Poison DoT is slightly lower than blades (ranged balance), but perfect for "Arcing" mode.
*   **Poison Types:**
    *   *Accumulative (Stacking):* (e.g., Belladonna). Each hit increases DoT or extends duration (up to a 3-stack cap). For long boss fights.
    *   *Acute (Single-shot):* (e.g., Viper Serum). Instant heavy damage on first hit. Reapplying does not stack, it only **refreshes the timer**. For burst damage and PvP.