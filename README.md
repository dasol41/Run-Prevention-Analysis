# Run Prevention & Pitch Strategy Analysis

## Overview

This project is a pitch-level run prevention case study analyzing a starting pitcher’s year-over-year arsenal evolution and its impact on bat-missing efficiency and matchup optimization.

Designed in the context of a professional baseball operations evaluation framework, this analysis emphasizes process-driven metrics and actionable strategic recommendations.

Using pitch-by-pitch data across two seasons (2024–2025), this analysis evaluates changes in pitch mix, pitch quality, and command intent. It develops a data-driven strategy for attacking a specific hitter profile.

---

## Objectives

- Quantify year-over-year pitch mix adjustments
- Measure bat-missing ability (Whiff%, CSW%)
- Evaluate command through zone & edge targeting
- Identify optimal put-away pitch strategy
- Develop matchup-specific game planning recommendations

---

## Data & Methodology

Pitch-level dataset including:
- Pitch type
- Swing / Whiff indicators
- Called strikes
- Chase indicators
- Zone classification (heart, shadow, etc.)
- Plate location coordinates

### Custom Metrics Engineered

- **Whiff%** = Whiffs / Swings  
- **CSW%** = (Called Strikes + Whiffs) / Total Pitches  
- **Chase Rate** = Chases / Swings  
- **Zone% / Edge%** for command evaluation  

Feature engineering was performed using Pandas to create advanced pitch outcome metrics aligned with modern Baseball Operations evaluation standards.

---

## Key Findings

### 1. Arsenal Evolution (2024 → 2025)

- Reduced sinker dependency
- Increased cutter and changeup usage
- Introduced sweeper and four-seam fastball
- Greater pitch mix diversification

This structural shift reflects a move toward a more swing-and-miss oriented approach.

---

### 2. Bat-Missing Efficiency

- Sweeper emerged as the most effective put-away pitch
- Sinker effective for early-count leverage, but limited finishing utility
- Four-seam best used for eye-level disruption rather than primary finisher

Pitch selection optimization suggests de-emphasizing sinkers in two-strike counts while leveraging sweepers in leverage situations.

---

### 3. Command Intent (Sweeper Location)

Location heat mapping shows:
- Consistent glove-side targeting
- Frequent expansion just off the plate
- Minimal heart-zone misses

This indicates deliberate chase-inducing usage rather than strike-stealing intent.

---

### 4. Matchup Strategy vs Hitter Profile

Hitter analysis revealed elevated whiff rates against:
- Sweepers
- Cutters
- Breaking pitches with lateral movement

Recommended Game Plan:

- Early Count: Cutter/Sinker edge targeting for strike leverage  
- Even Counts: Horizontal expansion with sweeper  
- Two-Strike: Sweeper primary put-away option  
- Occasional elevated four-seam for timing disruption  

This alignment maximizes pitcher strengths against hitter weaknesses to improve run prevention efficiency.

---

## Visualizations

### Pitch Mix Evolution
![Pitch Mix](visuals/pitch_mix_2024_2025.png)

### Pitcher Whiff% by Pitch Type (2025)
![Pitcher Whiff](visuals/pitcherB_whiff_2025.png)

### Hitter Whiff% by Pitch Type (2025)
![Hitter Whiff](visuals/playerA_whiff_2025.png)

### Sweeper Location Map
![Sweeper Location](visuals/pitcherB_sweeper_location_2025.png)

---

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Pitch-level feature engineering
- Custom baseball analytics metrics

---
## Author

Dasol Shin  
Computational & Data Sciences  
Baseball Analytics | Sports Data Science

