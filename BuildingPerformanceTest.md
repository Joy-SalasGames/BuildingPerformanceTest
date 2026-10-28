# Building Performance Test — Top 10 Offenders

**Source:** Frank, Oct 26  
**Tester:**  Joy    
**Test date:**  28 October 2026     
**Unity version:**  6000.3.11f1     
**Target platform:**  PC    
**Test environment:** Editor Play Mode  
**Resolution:**  1920x1080  
**Quality level:**  High

## Test Baseline

| Metric | Value |
|---|---:|
| Baseline draw calls | 17 |
| Baseline triangles | 2.335 |

## Results — Worst First

| Rank | Building | Building Draw Calls | Building Triangles | Screenshot |
|---:|---|---:|---:|---:|
| 1 |  |  |  | [View screenshot](LINK) |
| 2 |  |  |  | [View screenshot](LINK) |
| 3 |  |  |  | [View screenshot](LINK) |
| 4 |  |  |  | [View screenshot](LINK) |
| 5 |  |  |  | [View screenshot](LINK) |
| 6 |  |  |  | [View screenshot](LINK) |
| 7 |  |  |  | [View screenshot](LINK) |
| 8 |  |  |  | [View screenshot](LINK) |
| 9 |  |  |  | [View screenshot](LINK) |
| 10 |  |  |  | [View screenshot](LINK) |

## All Buildings by District

### Chinatown District

| No | Building | Building Draw Calls | Building Triangles | Screenshot |
|---:|---|---:|---:|---:|
| 1 | Building_1 | 54 | 20.086 | [View screenshot](https://github.com/Joy-SalasGames/BuildingPerformanceTest/blob/main/Screenshots/Chinatown/Building_1.png?raw=true) |
| 2 |  |  |  | [View screenshot](LINK) |
| 3 |  |  |  | [View screenshot](LINK) |
| 4 |  |  |  | [View screenshot](LINK) |
| 5 |  |  |  | [View screenshot](LINK) |
| 6 |  |  |  | [View screenshot](LINK) |
| 7 |  |  |  | [View screenshot](LINK) |
| 8 |  |  |  | [View screenshot](LINK) |
| 9 |  |  |  | [View screenshot](LINK) |
| 10 |  |  |  | [View screenshot](LINK) |

### Poor District & Working Class

| No | Building | Building Draw Calls | Building Triangles | Screenshot |
|---:|---|---:|---:|---:|
| 1 |  |  |  | [View screenshot](LINK) |
| 2 |  |  |  | [View screenshot](LINK) |
| 3 |  |  |  | [View screenshot](LINK) |
| 4 |  |  |  | [View screenshot](LINK) |
| 5 |  |  |  | [View screenshot](LINK) |
| 6 |  |  |  | [View screenshot](LINK) |
| 7 |  |  |  | [View screenshot](LINK) |
| 8 |  |  |  | [View screenshot](LINK) |
| 9 |  |  |  | [View screenshot](LINK) |
| 10 |  |  |  | [View screenshot](LINK) |

### Wealthy District

| No | Building | Building Draw Calls | Building Triangles | Screenshot |
|---:|---|---:|---:|---:|
| 1 |  |  |  | [View screenshot](LINK) |
| 2 |  |  |  | [View screenshot](LINK) |
| 3 |  |  |  | [View screenshot](LINK) |
| 4 |  |  |  | [View screenshot](LINK) |
| 5 |  |  |  | [View screenshot](LINK) |
| 6 |  |  |  | [View screenshot](LINK) |
| 7 |  |  |  | [View screenshot](LINK) |
| 8 |  |  |  | [View screenshot](LINK) |
| 9 |  |  |  | [View screenshot](LINK) |
| 10 |  |  |  | [View screenshot](LINK) |


## Calculation

```text
Building Draw Calls = Total Draw Calls - Baseline Draw Calls
Building Triangles  = Total Triangles - Baseline Triangles
```


## Test Conditions

- All buildings were tested individually in the same dedicated benchmark scene.
- Only the benchmark plane, required lighting, main camera, and one building were active during each test.
- Each building was placed at the same reference position and rotation, with its base aligned to the benchmark plane.
- Camera position, rotation, Field of View (FOV), projection type, and clipping planes remained unchanged throughout all tests.
- The camera was positioned to accommodate the largest building while maintaining consistent framing conditions.
- Resolution (1920×1080), quality level (High), render pipeline, lighting, and shadow settings remained unchanged.
- Static batching, GPU instancing, SRP Batcher, LOD, and occlusion culling settings were kept consistent with the project's configuration.
- Original building meshes, materials, renderer settings, and LOD configurations were not modified during testing.
- All measurements were performed using the same execution environment (Editor Play Mode or PC Build).
- The baseline was recorded using the benchmark scene without any building active.
- Each building was activated individually, and its rendering statistics were measured after the scene stabilized.
- Draw Calls and Triangles were recorded using exact numerical values without rounding or abbreviated notation.
- Building-specific values were calculated by subtracting the baseline from the total rendering statistics.
- Screenshots were captured from the same Game View configuration, showing the tested building and its rendering statistics.
- Buildings were ranked by their calculated Draw Calls, highest first. Ties were resolved using their calculated Triangles.
- Any visibility, clipping, LOD, or rendering anomalies were documented in the Notes section.

## Notes

| Building / Rank | Notes |
|---|---|
|  |  |
