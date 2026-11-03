# New Building Performance Test

**Tester:**  Joy    
**Test date:**  3 November2026     
**Unity version:**  6000.3.11f1     
**Target platform:**  PC    
**Test environment:** Editor Play Mode  
**Resolution:**  1920x1080  
**Quality level:**  High

## Test Baseline

| Metric | Value |
|---|---:|
| Baseline draw calls | 15 |
| Baseline triangles | 1.935 |

## Results

| Rank | Building | Building Draw Calls | Building Triangles | Screenshot |
|---:|---|---:|---:|---:|
| 1 | Building | 10 | 4.382 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Building.png) |
| 2 | Building_2 | 60 | 33.074 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Building_2.png) |
| 3 | Building_3 | 26 | 14.990 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Building_3.png) |
| 4 | Mahjong | 22 | 7.310 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Mahjong.png) |
| 5 | Sapporo Ramen | 8 | 3.440 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Sapporo_Ramen.png) |
| 6 | Yong Tai Building | 32 | 20.574 | [View screenshot](https://raw.githubusercontent.com/Joy-SalasGames/BuildingPerformanceTest/refs/heads/oct-11/Screenshots/Yong_Tai_Building.png) |

## Calculation

```text
Building Draw Calls = Total Draw Calls - Baseline Draw Calls
Building Triangles  = Total Triangles - Baseline Triangles
```


## Test Conditions

- All buildings were tested individually in the same dedicated benchmark scene.
- Only the benchmark required lighting, main camera, and one building were active during each test.
- Each building was placed at the same reference position and rotation, with its base aligned to the benchmark position.
- Camera position, rotation, Field of View (FOV), projection type, and clipping planes remained unchanged throughout all tests.
- Resolution (1920×1080), quality level (High), render pipeline, lighting, and shadow settings remained unchanged.
- Static batching, GPU instancing, SRP Batcher, LOD, and occlusion culling settings were kept consistent with the project's configuration.
- Original building meshes, materials, renderer settings, and LOD configurations were not modified during testing.
- All buildings had their main geometry merged into a single mesh. Fake interiors remained as separate, unmerged meshes within their respective building's child hierarchy.
- All measurements were performed using the same execution environment (Editor Play Mode).
- The baseline was recorded using the benchmark scene without any building active.
- Each building was activated individually, and its rendering statistics were measured after the scene stabilized.
- Draw Calls and Triangles were recorded using exact numerical values without rounding or abbreviated notation.
- Building-specific values were calculated by subtracting the baseline from the total rendering statistics.
- Screenshots were captured from the same Game View configuration, showing the tested building and its rendering statistics.
- Buildings were ranked by their calculated Draw Calls, highest first. Ties were resolved using their calculated Triangles.
- Any visibility, clipping, LOD, or rendering anomalies were documented in the Notes section.
