# Дебаффы и Статусы / Debuffs & Status Effects

## 🇷🇺 Русский

### Философия: Мгновенное считывание и Точность
В динамичном бою игрок должен мгновенно оценивать угрозу, но при этом иметь доступ к точным цифрам. Система построена на комбинации **формы (иконка)**, **цвета (рамка угрозы)** и **текста (процент под иконкой)**.

### 1. Типы дебаффов (Иконки)
Каждый статус имеет уникальную, легко узнаваемую иконку:
1. **Огонь (Горение):** Иконка пламени.
2. **Лёд (Обморожение/Замедление):** Иконка снежинки.
3. **Кровотечение:** Иконка капли крови.
4. **Яд:** Иконка змеи.
5. **Потеря контроля (Стан/Хаос):** Иконка перечеркнутой ноги или разбитого черепа.

### 2. Визуальное отображение и Сила эффекта (Severity Tiers)
Каждый дебафф отображается в виде **иконки**, под которой **четким, контрастным шрифтом указан процент** (например, "5%"). Контур иконки меняет цвет для мгновенной оценки угрозы издалека:

*   🟡 **Светло-желтый (Легкий):** 
    *   *Отображение:* Иконка + "1.5% - 3.8%" (для DoT) или "до 10%" (для замедления).
*   🟠 **Ярко-желтый / Оранжевый (Средний):** 
    *   *Отображение:* Иконка + "4% - 6.5%" (для DoT) или "до 17%" (для замедления).
*   🔴 **Светло-красный (Мощный):** 
    *   *Отображение:* Иконка + "6.6% - 7.5%" (для DoT) или "до 22%" (для замедления).
*   🟥 **Багрово-красный (Эпический):** 
    *   *Отображение:* Иконка + "7.6% - 10%" (для DoT) или "до 27%" (для замедления).

### 3. Особое правило для Потери контроля
Стан, очарование или любая другая форма потери контроля — это **бинарное состояние** (ты либо управляешь персонажем, либо нет). 
*   Иконка потери контроля **всегда имеет один нейтральный цвет** (серебристый или белый) и сопровождается коротким, четким таймером вместо процента.
*   Цветовая градация к ней не применяется, так как даже 1 секунда хаоса или атаки по своим фатальна. Игрок должен видеть только время: "3.0с".

### 4. Механика Обморожения (Важная сноска)
Любой тип замедления в игре визуально и механически трактуется как **Обморожение**. 
*   **Физический упадок:** Замедляется *всё* физическое: ходьба, скорость атаки, кувырки и время накладывания повязки.
*   **Взаимодействие с магией:** Физическое онемение *не влияет* на скорость произнесения заклинаний.
*   **Осечки от холода:** Однако замерзание нарушает ментальную концентрацию. При дебаффе Обморожения заклинания начинают давать **осечки (Misfire)** — особенно с длительным временем каста. Чем сильнее обморожение (выше %), тем выше шанс, что заклинание развеется без урона.

---

## 🇬🇧 English

### Philosophy: Instant Readability & Precision
In dynamic combat, players must instantly assess threats while having access to exact numbers. The system is built on a combination of **shape (icon)**, **color (threat border)**, and **text (percentage below the icon)**.

### 1. Debuff Types (Icons)
Each status has a unique, easily recognizable icon:
1. **Fire (Burn):** Flame icon.
2. **Ice (Frostbite/Slow):** Snowflake icon.
3. **Bleeding:** Blood drop icon.
4. **Poison:** Snake icon.
5. **Loss of Control (Stun/Chaos):** Crossed-out leg or shattered skull icon.

### 2. Visual Display & Severity Tiers
Each debuff is displayed as an **icon** with the **percentage value clearly written below it** (e.g., "5%"). The icon's border changes color for instant threat assessment from a distance:

*   🟡 **Light Yellow (Minor):** 
    *   *Display:* Icon + "1.5% - 3.8%" (for DoT) or "up to 10%" (for slow).
*   🟠 **Bright Yellow / Orange (Moderate):** 
    *   *Display:* Icon + "4% - 6.5%" (for DoT) or "up to 17%" (for slow).
*   🔴 **Light Red (Severe):** 
    *   *Display:* Icon + "6.6% - 7.5%" (for DoT) or "up to 22%" (for slow).
*   🟥 **Crimson Red (Epic):** 
    *   *Display:* Icon + "7.6% - 10%" (for DoT) or "up to 27%" (for slow).

### 3. Special Rule for Loss of Control
Stun, charm, or any other form of loss of control is a **binary state** (you either control the character or you don't).
*   The loss of control icon **always has one neutral color** (silver or white) and is accompanied by a short, clear timer instead of a percentage.
*   Color grading does not apply, as even 1 second of chaos or friendly fire is fatal. The player only needs to see the time: "3.0s".

### 4. Frostbite Mechanics (Important Note)
Any type of slowing effect in the game is visually and mechanically treated as **Frostbite**.
*   **Physical Decay:** *All* physical actions are slowed: walking, attack speed, dodge rolls, and bandaging time.
*   **Interaction with Magic:** Physical numbness does *not* affect spell casting speed.
*   **Cold Misfires:** However, freezing disrupts mental concentration. With the Frostbite debuff, spells begin to **Misfire** — especially those with long cast times. The higher the frostbite percentage, the higher the chance the spell dissipates without dealing damage.