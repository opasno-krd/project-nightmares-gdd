# ИИ Мобов, Аггро и Тактика Боя / Mob AI, Aggro & Combat Tactics

## 🇷🇺 Русский

### Философия: Тактическая Бойня, а не "Тык-Тык"
Бой в игре напоминает жестокие, тактические схватки (в духе *No Rest for the Wicked*). Это не обмен цифрами урона, а управление дистанцией, стаминой, позиционированием и прерывание действий врага. Мобы — умные тактические единицы, а не болванки на привязи.

### 1. Обнаружение и Инициация Боя
*   **Визуальный радиус:** 15-20 метров. В этом радиусе моб видит игрока и начинает атаку.
*   **Аудиальный радиус (Шум):** 30-40 метров. Если игрок шумит (спринт, тяжелая броня, громкие заклинания), мобы за пределами видимости переходят в режим "Заинтересованности" и начинают медленно и неспешно подходить к источнику звука, сужая кольцо окружения.

### 2. Механика Вызова Подмоги (Расстояние + Время)
Чтобы удержать моба в фокусе, игрок должен наносить урон или находиться в радиусе 3 метров хотя бы раз в 5 секунд, не отходя дальше чем на 8 метров. 
Если условия нарушены, моб пытается позвать подмогу. Способ зависит от типа существа:
*   **Люди/Гуманоиды:** Издают громкий крик. Все союзники в радиусе 30 метров получают алерт и бегут на помощь.
*   **Звери:** Физически бегут за ближайшими сородичами, приводя их к игроку.
*   **Духи/Нежить:** Мистический призыв. Все нематериальные существа в радиусе 50 метров мгновенно телепортируются или материализуются рядом. 
*   **Важно:** Эта механика **не работает на боссов**. Боссы не зовут подмогу таким образом (их механики прописаны индивидуально).

### 3. Динамическая Система Приоритетов (Threat Priority)
Мобы выбирают цель на основе динамической цифры приоритета. Чем она выше, тем агрессивнее моб атакует эту цель.

*   **Базовый приоритет:** Уровень персонажа.
*   **Таунт (Крик-Оскорбление):** +100 к приоритету. Работает *только* на разумных существах, понимающих речь. Длится 5-10 секунд.
*   **Конец таунта:** -100 к приоритету. Моб "скучает", отвлекается и переключается на более актуальную угрозу.
*   **Каст лечения:** +70 к приоритету. Мобы понимают, что устранение источника восстановления HP критически важно.

### 4. Механика Хила: Баланс Риска и Подготовки
Хилер — это не "фабрика HP", как в старых MMO. Лечение строго ограничено ресурсами и временем каста.

*   **Экстренный хил (В бою):** 
    *   Быстрый каст. Восстанавливает фиксированные **35% HP** за 2 очень коротких тика (по 0.5 сек).
    *   *Цена:* Огромный расход маны. Обычный клерик может позволить себе максимум 2 таких каста за весь бой.
    *   *Риск:* Дает +70 к приоритету, делая хилера главной целью.
*   **Медитативный хил (Вне боя):**
    *   Медленный каст (7 секунд). Восстанавливает **5% HP каждые 2 секунды** (всего 20 тиков = 100% HP).
    *   *Уязвимость:* Если каст прерван (получен урон, начат бой), хилер мгновенно получает **1000% аггро** от всех мобов вокруг, а каст сбивается.
    *   *Тактический хак ("Pre-cast"):* Опытные игроки начинают кастовать этот 7-секундный хил *за секунду до вступления в бой*. Если каст завершается успешно, хилер входит в бой с постоянным тиком восстановления, который сложно прервать, не фокуся его в первую очередь.

### 5. Реакция Мобов на Роли в Пати
*   **На Танка:** Мобы не "прилипают" к нему. Они постоянно кружат вокруг, пытаясь зайти за спину или с фланга, чтобы сорвать фокус для тяжелых атак. Танк должен физически перекрывать им путь и использовать таунт.
*   **На Лучника:** Мобы пытаются укрыться за препятствиями (деревья, камни). Если не могут — сокращают дистанцию рывком. Если лучник отступает, они бегут звать подмогу.
*   **На Кастера (Мага):** Если маг один, мобы бьют его в ближнем бою, экономя ману. Если магов 2+, мобы начинают спамить своими спеллами в приоритетную цель, пытаясь перекастовать мага.

---

## 🇬🇧 English

### Philosophy: Tactical Brawl, Not "Click-Click"
Combat resembles brutal, tactical skirmishes (akin to *No Rest for the Wicked*). It's not about trading damage numbers, but managing distance, stamina, positioning, and interrupting enemies. Mobs are smart tactical units, not tethered dummies.

### 1. Detection & Initiation
*   **Visual Radius:** 15-20 meters. The mob sees the player and initiates combat.
*   **Auditory Radius (Noise):** 30-40 meters. If the player makes noise (sprinting, heavy armor, loud spells), mobs outside visual range enter "Interest" mode and slowly approach the sound source, tightening the encirclement.

### 2. Reinforcement Mechanics (Distance + Time)
To keep a mob focused, the player must deal damage or stay within 3 meters at least once every 5 seconds, without moving further than 8 meters away. 
If conditions are violated, the mob calls for help. The method depends on the creature type:
*   **Humans/Humanoids:** Yell loudly. All allies within 30 meters get an alert and run to help.
*   **Beasts:** Physically run to fetch nearby kin, leading them to the player.
*   **Spirits/Undead:** Mystical summoning. All non-material beings within 50 meters instantly teleport or materialize nearby.
*   **Important:** This mechanic **does not work on Bosses**. Bosses do not call reinforcements this way (their mechanics are scripted individually).

### 3. Dynamic Threat Priority System
Mobs choose targets based on a dynamic priority number. The higher it is, the more aggressively the mob attacks that target.

*   **Base Priority:** Character level.
*   **Taunt (Insulting Shout):** +100 priority. Works *only* on intelligent beings that understand speech. Lasts 5-10 seconds.
*   **Taunt Ends:** -100 priority. The mob gets "bored", gets distracted, and switches to a more relevant threat.
*   **Healing Cast:** +70 priority. Mobs understand that eliminating the source of HP recovery is critical.

### 4. Healing Mechanics: Risk vs. Preparation Balance
The healer is not an "HP factory" like in old MMOs. Healing is strictly limited by resources and cast time.

*   **Emergency Heal (In Combat):**
    *   Fast cast. Restores a fixed **35% HP** over 2 very short ticks (0.5 sec each).
    *   *Cost:* Huge mana drain. A standard cleric can afford a maximum of 2 such casts per entire fight.
    *   *Risk:* Grants +70 priority, making the healer the primary target.
*   **Meditative Heal (Out of Combat):**
    *   Slow cast (7 seconds). Restores **5% HP every 2 seconds** (total 20 ticks = 100% HP).
    *   *Vulnerability:* If the cast is interrupted (damage taken, combat starts), the healer instantly gains **1000% aggro** from all nearby mobs, and the cast is canceled.
    *   *Tactical Hack ("Pre-cast"):* Experienced players start casting this 7-second heal *a second before engaging*. If the cast completes successfully, the healer enters combat with a constant healing tick that is hard to interrupt without focusing them down immediately.

### 5. Mob Reactions to Party Roles
*   **To the Tank:** Mobs don't "stick" to them. They constantly circle, trying to get behind or flank to disrupt heavy attack focus. The tank must physically block their path and use taunts.
*   **To the Archer:** Mobs try to take cover behind obstacles (trees, rocks). If unable, they close the distance with a dash. If the archer retreats, they run to call reinforcements.
*   **To the Caster (Mage):** If there's only one mage, mobs melee them to save mana. If there are 2+ mages, mobs start spamming their own spells at the priority target, trying to out-cast the mage.