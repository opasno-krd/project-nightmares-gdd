# Технические Спецификации / Technical Specifications

## 🇷🇺 Русский

### Философия: Классика встречает Современные Стандарты
Игра сочетает в себе хардкорные механики классических RPG с современной визуальной подачей и надежной сетевой архитектурой, защищающей экономику.

### 1. Игровой Движок: Unreal Engine 5 (UE5)
*   **Nanite:** Виртуализированная геометрия. Позволяет использовать высокодетализированные модели (ржавые латы, сюрреалистичных монстров, детализированные руины) без потери производительности.
*   **Lumen:** Динамическое глобальное освещение. Критически важно для создания мрачной, давящей атмосферы хоррора и четкого визуального разделения света и тени в бою.
*   **World Partition:** Система бесшовной загрузки больших открытых миров. Позволяет реализовать плавные переходы между зонами (Дикие Земли -> Город) без загрузочных экранов, сохраняя высокую производительность.

### 2. Сетевая Архитектура: Авторитарный Сервер (Authoritative Server)
*   **Принцип:** Сервер является единственным источником истины. Клиент (игра игрока) только отправляет намерения (нажал кнопку атаки), а сервер рассчитывает попадание, урон и дроп.
*   **Зачем это нужно:** Это **фундаментальная защита** от читов, ботов и RMT. Невозможно подделать дроп книги, ускорить перемещение или нанести урон сквозь стены, так как сервер это проверит и отвергнет.
*   **Client-Side Prediction:** Для сохранения плавности управления (особенно при кувырках и кастах) клиент предсказывает движение, но окончательное решение всегда за сервером.

### 3. Визуальный Стиль и Читаемость (Visual Readability)
*   **Высокий Контраст:** Несмотря на мрачный сеттинг (Dark Fantasy), враги и интерактивные объекты должны иметь четкие, читаемые силуэты на фоне окружения.
*   **Визуальная обратная связь (VFX):** Атаки боссов (например, конус удара Плюшевого Медведя или зона приземления Копитана) должны иметь четкие, контрастные визуальные маркеры за 0.5–1 секунду до удара, чтобы игрок мог реагировать на скилл, а не на удачу.

### 4. Оптимизация и Платформы
*   **Целевая платформа:** PC (Windows).
*   **Методы оптимизации:** 
    *   Агрессивный Occlusion Culling (не рендерить то, что за стеной).
    *   Динамическое снижение качества теней и эффектов при большом скоплении мобов (например, при призыве подмоги или в фазе с моряками-духами).
    *   Строгий лимит полигонов для массовых NPC (караваны, стража).

---

## 🇬🇧 English

### Philosophy: Classic Meets Modern Standards
The game combines hardcore classic RPG mechanics with modern visual presentation and robust network architecture designed to protect the economy.

### 1. Game Engine: Unreal Engine 5 (UE5)
*   **Nanite:** Virtualized geometry. Allows the use of highly detailed models (rusty plate armor, surreal monsters, detailed ruins) without performance loss.
*   **Lumen:** Dynamic global illumination. Critically important for creating a grim, oppressive horror atmosphere and clear visual separation of light and shadow in combat.
*   **World Partition:** Seamless open-world loading system. Allows smooth transitions between zones (Wilds -> City) without loading screens while maintaining high performance.

### 2. Network Architecture: Authoritative Server
*   **Principle:** The server is the single source of truth. The client (player's game) only sends intentions (pressed attack button), while the server calculates hits, damage, and loot.
*   **Why it's needed:** This is the **fundamental protection** against cheats, bots, and RMT. It is impossible to fake a book drop, speed hack, or hit through walls, as the server will validate and reject it.
*   **Client-Side Prediction:** To maintain smooth controls (especially for dodges and casts), the client predicts movement, but the final decision always rests with the server.

### 3. Visual Style & Readability
*   **High Contrast:** Despite the grim Dark Fantasy setting, enemies and interactive objects must have clear, readable silhouettes against the environment.
*   **Visual Feedback (VFX):** Boss attacks (e.g., the Plush Bear's cone strike or the Captain's landing zone) must have clear, high-contrast visual markers 0.5–1 second before impact, allowing players to react based on skill, not luck.

### 4. Optimization & Platforms
*   **Target Platform:** PC (Windows).
*   **Optimization Methods:**
    *   Aggressive Occlusion Culling (do not render what is behind a wall).
    *   Dynamic scaling of shadow and effect quality during high mob density (e.g., during reinforcement calls or the ghost sailor phase).
    *   Strict polygon limits for mass NPCs (caravans, city guards).