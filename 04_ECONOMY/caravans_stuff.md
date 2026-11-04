# Механика Тюков, Караванов и Защита от Эксплойтов / Bales, Caravans & Anti-Exploit Mechanics

## 🇷🇺 Русский

Этот документ описывает физическую реализацию логистики и меры по предотвращению злоупотреблений (anti-griefing/anti-exploit) в системе караванов.

### 1. Тюки как физические объекты (Bales as Physical Objects)
Тюки с ресурсами (руда, скрап, редкие материалы) — это **физические 3D-объекты** в мире игры, а не абстрактные цифры в инвентаре.

*   **Физика и Коллизия:** Тюк имеет физическую модель. Его нельзя «спрятать» в текстуры или недоступные места.
*   **Ограничения переноса:** Игрок может нести максимум 1-2 тюка. При этом накладывается дебафф **«Перегруз»**: скорость -50%, запрет на использование планера, запрет на кувырки, урон в ближнем бою -30%.
*   **Слот экипировки:** Тюк занимает слот «руки» (как двуручное оружие). Игрок не может одновременно нести тюк и атаковать.
*   **Таймер исчезновения:** Выброшенный тюк исчезает через 5 минут, если не установлен на повозку или в сундук.

### 2. Механика Эскорта Каравана (Caravan Escort Mechanics)
Игрок не тащит груз на себе (как в казуальных MMO). Караван — это **повозка с NPC-водителем и вьючными животными**. Игрок выступает эскортом.

*   **Радиус эскорта:** Игрок должен находиться в радиусе 10-15 метров от каравана. Если игрок отстает на 20+ метров, караван останавливается.
*   **Смерть эскорта:** Если игрок-эскорт умирает, караван продолжает движение, но **теряет 10% груза** (NPC-водитель паникует и роняет тюки).
*   **Ограничения управления:** Игрок не может «сесть» на повозку, ускорить её заклинаниями или управлять животными. Это исключает клиентские эксплойты скорости.

### 3. Ограбление каравана: Риск и Награда (Caravan Robbery: Risk & Reward)
Нападение на караван возможно, но система делает его экономически рискованным.

*   **Механика атаки:** Нападающий должен убить NPC-водителя (у него есть HP и базовая защита). После смерти водителя караван останавливается, тюки выпадают на землю.
*   **Окно ограбления:** 60 секунд. После этого караван телепортируется обратно в город с оставшимся грузом.
*   **Последствия для грабителя:**
    1.  Получает статус **«Вне Закона» (Outlaw)** на 1 час. Стража атакует при виде.
    2.  Поднятые тюки помечаются как **«Украденные»**. Их нельзя продать легальным вендорам (только на черном рынке с комиссией 50%).
    3.  Если грабитель убит эскортом в течение 5 минут после ограбления, **все тюки возвращаются каравану**.

### 4. Прогрессивные лимиты и Клановые караваны (Progressive Limits & Clan Caravans)
*   **Прогрессивные лимиты:** Передача ресурсов между игроками ограничена системой «Уз» (Bonds). Новичок (0 часов совместной игры) может передать только 10 единиц руды. Ветеран (50+ часов) — 1000 единиц.
*   **Защита от ботов:** Для прокачки «Уз» требуется реальный *combat contribution* (урон, хил, ассист). АФК-фермы не получают прогресс.
*   **Клановые караваны:** Клан может создать официальный караван с логотипом (до 50 тюков). Нападение на него объявляет **войну кланам**, что влечет за собой потерю репутации и возможность осады клан-холла.

### 5. Защита от эксплойтов (Red Teaming / Anti-Exploit Q&A)
*   **"Я могу спрятать тюк в текстуры"** → Тюки имеют строгую физическую коллизию. Таймер исчезновения 5 минут.
*   **"Я могу передать тюк без системы"** → Прямая передача запрещена. Только через сундук или повозку. Все транзакции логируются.
*   **"Я могу убить караван и забрать всё без риска"** → Статус Outlaw, помеченные тюки, невозможность продать легально. ROI (возврат инвестиций) отрицательный.
*   **"Я могу использовать баги физики/ускорения"** → Авторитарный сервер (Authoritative Server). Все действия валидируются на сервере. Клиентские баги не проходят.

---

## 🇬🇧 English

This document describes the physical implementation of logistics and anti-griefing/anti-exploit measures in the caravan system.

### 1. Bales as Physical Objects
Bales of resources (ore, scrap, rare materials) are **physical 3D objects** in the game world, not abstract inventory numbers.

*   **Physics & Collision:** Bales have a physical mesh. They cannot be "hidden" in textures or inaccessible areas.
*   **Carry Limits:** A player can carry a maximum of 1-2 bales. This applies the **"Overload" debuff**: -50% speed, glider disabled, dodging disabled, melee damage -30%.
*   **Equipment Slot:** A bale occupies the "hand" slot (like a two-handed weapon). The player cannot carry a bale and attack simultaneously.
*   **Despawn Timer:** A dropped bale disappears after 5 minutes if not placed on a cart or in a chest.

### 2. Caravan Escort Mechanics
The player does not carry the load on their back (like in casual MMOs). A caravan is a **cart with an NPC driver and pack animals**. The player acts as an escort.

*   **Escort Radius:** The player must stay within 10-15 meters of the caravan. If the player falls behind by 20+ meters, the caravan stops.
*   **Escort Death:** If the escorting player dies, the caravan continues but **loses 10% of its cargo** (the NPC driver panics and drops bales).
*   **Control Limits:** The player cannot "ride" the cart, speed it up with spells, or control the animals. This eliminates client-side speed exploits.

### 3. Caravan Robbery: Risk & Reward
Attacking a caravan is possible, but the system makes it economically risky.

*   **Attack Mechanic:** The attacker must kill the NPC driver (who has HP and basic defense). Upon the driver's death, the caravan stops, and bales drop to the ground.
*   **Looting Window:** 60 seconds. After this, the caravan teleports back to the city with the remaining cargo.
*   **Consequences for the Robber:**
    1.  Gains **"Outlaw" status** for 1 hour. City guards attack on sight.
    2.  Looted bales are marked as **"Stolen"**. They cannot be sold to legal vendors (only on the black market with a 50% commission).
    3.  If the robber is killed by the escort within 5 minutes of the robbery, **all bales are returned to the caravan**.

### 4. Progressive Limits & Clan Caravans
*   **Progressive Limits:** Resource transfer between players is limited by the "Bonds" system. A newbie (0 hours of joint play) can transfer only 10 units of ore. A veteran (50+ hours) — 1000 units.
*   **Anti-Bot Protection:** Leveling up "Bonds" requires real *combat contribution* (damage, healing, assists). AFK farms do not gain progress.
*   **Clan Caravans:** A clan can create an official caravan with a clan logo (up to 50 bales). Attacking it declares **war on the clans**, resulting in reputation loss and potential clan hall sieges.

### 5. Anti-Exploit Q&A (Red Teaming)
*   **"I can hide a bale in textures"** → Bales have strict physical collision. 5-minute despawn timer.
*   **"I can transfer a bale outside the system"** → Direct transfer is forbidden. Only via chests or carts. All transactions are logged.
*   **"I can kill the caravan and take everything risk-free"** → Outlaw status, marked bales, inability to sell legally. Negative ROI.
*   **"I can use physics/speed bugs"** → Authoritative Server. All actions are validated server-side. Client-side bugs do not pass.