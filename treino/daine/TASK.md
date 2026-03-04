# Task: Build Daine Cavalcanti's Training Page

Modify `index.html` (copied from Rosane's template) to create Daine's personalized training page.

## Student Info
- **Name:** Daíne Cavalcanti da Silva
- **Goal:** Emagrecimento (weight loss)
- **Split:** ABC, 3x/week (Seg A, Qua B, Sex C)
- **Sets/Reps:** 3x15-20
- **Restrictions:** Protrusão discal L5, Escoliose, Hipotireoidismo Hashimoto. No barbell on back, no deep squats, no Bulgarian, no Lateral Raise.

## Changes Required

### 1. Update all references from "Rosane" to "Daine"
- Title, header, localStorage keys (`maxresults-daine-*`), all name mentions

### 2. Schedule: ABC 3x/week
Days array should be:
```
Seg → Treino A (Anterior + MaxLift B&T)
Ter → Descanso
Qua → Treino B (Posterior + MaxLift B&T)  
Qui → Descanso
Sex → Treino C (Full Body)
Sáb → Descanso
```

### 3. TREINO A — Anterior + MaxLift Bíceps & Tríceps

**Aquecimento Articular (warmup type):**
- Balanço Frontal das Pernas (1x12) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/d508q2wlkh_opt.mp4`
- Giros dos Braços Frente e Trás (1x12) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/8d76rg3vbsm_opt.mp4`

**Aquecimento Muscular (warmup type, different color/label):**
- Supino Reto com Halteres leve (2x20) — video: `https://vd.mfitpersonal.com.br/205/mp4/205.mp4`
  - Note: "Carga leve — apenas para aquecer"
- Leg Press 45° leve (2x20) — video: `https://vd.mfitpersonal.com.br/481/mp4/481.mp4`
  - Note: "Carga leve — apenas para aquecer"

**Mobilidade (mobility type):**
- Alongamento Peitoral (1x25s) — video YouTube: `be0xXepDGhQ`
- Alongamento de Coxa I (1x25s) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/lpgl41gg1op_opt.mp4`
- Alongamento Flexor do Quadril (1x25s) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/5e9lix657lb_opt.mp4`

**Bi-Set 1:**
- Leg Press 45° (3x15-20) — video: `https://vd.mfitpersonal.com.br/481/mp4/481.mp4`
- Supino Reto com Barra (3x15-20) — video: `https://vd.mfitpersonal.com.br/203/mp4/203.mp4`

**Bi-Set 2:**
- Cadeira Extensora (3x15-20) — video: `https://vd.mfitpersonal.com.br/504/mp4/504.mp4`
- Crucifixo Máquina (3x15-20) — video: `https://vd.mfitpersonal.com.br/530/mp4/530.mp4`

**Bi-Set 3:**
- Adução de Quadril Máquina (3x15-20) — video: `https://vd.mfitpersonal.com.br/514/mp4/514.mp4`
- Desenvolvimento com Halteres Neutro (3x15-20) — video: `https://vd.mfitpersonal.com.br/155/mp4/155.mp4`

**MaxLift (lift type):**
- MaxLift Mix 2 — Bíceps e Tríceps — video link (OneDrive): `https://1drv.ms/v/c/437d19de9d024724/IQAkRwKd3hl9IIBD5-MAAAAAATY48VJYTyzfx0Gq6gLKC2s?e=37FE2V`
  - This is NOT an MFIT video. Render as an external link button "▶ MaxLift Mix 2 — Bíceps e Tríceps" that opens in new tab.

**Cardio (cardio type):**
- Bike Spinning — video: `https://vd.mfitpersonal.com.br/527/mp4/527.mp4`

**Alongamento Final (stretching type):**
- Alongamento Peitoral (1x10s) — video YouTube: `be0xXepDGhQ`
- Alongamento de Coxa I (1x10s) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/lpgl41gg1op_opt.mp4`
- Alongamento Flexor do Quadril (1x10s) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/5e9lix657lb_opt.mp4`

### 4. TREINO B — Posterior + MaxLift Bíceps & Tríceps

**Aquecimento Articular:**
- Balanço Frontal das Pernas (1x12)
- Giros dos Braços Frente e Trás (1x12)

**Aquecimento Muscular:**
- Inclinação Frontal do Tronco com Halteres (1x15) — video: `https://vd.mfitpersonal.com.br/269/mp4/269.mp4` (Good Morning / Bom Dia)
  - Note: "Carga leve — apenas para aquecer"
- Remada Curvada leve (1x15) — video: `https://vd.mfitpersonal.com.br/565/mp4/565.mp4`
  - Note: "Carga leve — apenas para aquecer"

**Mobilidade:**
- Hand to Toes (1x25 reps + 20s embaixo) — video YouTube: `eFGc-g-HudQ`
  - Note: "25 repetições + segurar 20 segundos na posição inferior"
- Alongamento de Glúteos II (1x25s) — video: `https://vd.mfitpersonal.com.br/83/mp4/83.mp4`

**Bi-Set 1:**
- Cadeira Flexora (3x15-20) — video: `https://vd.mfitpersonal.com.br/502/mp4/502.mp4`
- Puxada Frontal (3x15-20) — video: `https://vd.mfitpersonal.com.br/565/mp4/565.mp4`

**Bi-Set 2:**
- Glúteos Coice na Polia (3x15-20) — video: `https://vd.mfitpersonal.com.br/457/mp4/457.mp4`
- Remada Baixa (3x15-20) — video: `https://vd.mfitpersonal.com.br/567/mp4/567.mp4`

**Bi-Set 3:**
- Abdução de Quadril Máquina (3x15-20) — video: `https://vd.mfitpersonal.com.br/515/mp4/515.mp4`
- Crucifixo Inverso Máquina (3x15-20) — video: `https://vd.mfitpersonal.com.br/531/mp4/531.mp4`

**MaxLift:**
- MaxLift Mix 2 — Bíceps e Tríceps (same OneDrive link as Treino A)

**Cardio:**
- Bike Spinning

**Alongamento Final:**
- Hand to Toes (1x10s) — video YouTube: `eFGc-g-HudQ`
- Alongamento de Glúteos II (1x10s) — video: `https://vd.mfitpersonal.com.br/83/mp4/83.mp4`

### 5. TREINO C — Full Body (musculação pura)

**Aquecimento Articular:**
- Balanço Frontal das Pernas (1x12)
- Giros dos Braços Frente e Trás (1x12)

**Aquecimento Muscular:**
- Supino Reto com Halteres leve (2x20) — video: `https://vd.mfitpersonal.com.br/205/mp4/205.mp4`
- Inclinação Frontal do Tronco com Halteres (1x15) — video: `https://vd.mfitpersonal.com.br/269/mp4/269.mp4`
- Agachamento Livre sem barra (2x20) — video: `https://vd.mfitpersonal.com.br/52/mp4/52.mp4`
  - Note: "Amplitude menor — sentar no banco como referência"

**Mobilidade:**
- Alongamento Peitoral (1x25s) — video YouTube: `be0xXepDGhQ`
- Alongamento de Coxa I (1x25s) — video: `https://d2vfutiy2j6sqj.cloudfront.net/13341/mp4/lpgl41gg1op_opt.mp4`
- Hand to Toes (1x25 reps + 20s) — video YouTube: `eFGc-g-HudQ`
- Alongamento de Glúteos II (1x25s) — video: `https://vd.mfitpersonal.com.br/83/mp4/83.mp4`

**Bi-Set 1:**
- Leg Press 45° (3x15-20) — video: `https://vd.mfitpersonal.com.br/481/mp4/481.mp4`
- Supino Reto com Barra (3x15-20) — video: `https://vd.mfitpersonal.com.br/203/mp4/203.mp4`

**Bi-Set 2:**
- Cadeira Flexora (3x15-20) — video: `https://vd.mfitpersonal.com.br/502/mp4/502.mp4`
- Puxada Frontal (3x15-20) — video: `https://vd.mfitpersonal.com.br/565/mp4/565.mp4`

**Bi-Set 3:**
- Cadeira Extensora (3x15-20) — video: `https://vd.mfitpersonal.com.br/504/mp4/504.mp4`
- Desenvolvimento com Halteres Neutro (3x15-20) — video: `https://vd.mfitpersonal.com.br/155/mp4/155.mp4`

**Bi-Set 4:**
- Glúteos 4 Apoios Caneleira (3x15-20) — video: `https://vd.mfitpersonal.com.br/240/mp4/240.mp4`
- Rosca Direta com Halteres (3x15-20) — video: `https://vd.mfitpersonal.com.br/109/mp4/109.mp4`

**Bi-Set 5:**
- Tríceps Corda (3x15-20) — video: `https://vd.mfitpersonal.com.br/418/mp4/418.mp4`
- Abdominal Supra (3x15-20) — video: `https://vd.mfitpersonal.com.br/20/mp4/20.mp4`

**Cardio:**
- Bike Spinning

**Alongamento Final:**
- Alongamento Peitoral (1x10s) — video YouTube: `be0xXepDGhQ`
- Alongamento de Coxa I (1x10s) 
- Hand to Toes (1x10s)
- Alongamento de Glúteos II (1x10s)

### 6. Important UI Details

- **YouTube videos:** For video IDs like `be0xXepDGhQ` and `eFGc-g-HudQ`, render as YouTube embeds or link buttons (not MFIT video player). Format: `https://www.youtube.com/watch?v=VIDEO_ID`
- **OneDrive MaxLift links:** Render as a prominent button with amber/gold color that opens in new tab. NOT as inline video.
- **Exercise videos:** All MFIT videos (URLs starting with `https://vd.mfitpersonal.com.br/` or `https://d2vfutiy2j6sqj.cloudfront.net/`) should use the existing inline video player from the template.
- **Rest time field (⏱ seg):** Keep the editable rest time input between bi-sets (from template).
- **Load fields:** Keep editable load fields for each exercise.
- **Avatar photo:** Keep the editable avatar (localStorage).
- **Dynamic week dates:** Keep the auto-calculating week dates.
- **Timer + frequency report:** Include the session timer (start/stop) and frequency report from Yasmin's page if present in template; if not present, add it.
- **Health alert:** Add a subtle warning banner at top: "⚠️ Protrusão discal L5 + Escoliose — Evitar sobrecarga na coluna"
- **Block types/colors:** Keep the same color scheme as template:
  - warmup = pink/rose accent
  - mobility = purple accent  
  - lift (bi-sets) = amber accent
  - maxlift = amber accent (distinct style for external link)
  - cardio = cyan accent
  - stretching = use mobility purple or a calm green

### 7. DO NOT change the overall visual design, CSS variables, fonts, or layout structure. Only change the workout data/content.
