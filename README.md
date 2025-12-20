# Dataset (JSON)

This repository provides the dataset used in the paper:

**“A Two-Stage Solution Incorporating Large Neighborhood Search for the Priority-Aware 2D Bin Packing Problem in Furniture Manufacturing”.**

All instances are stored in **JSON** format. File names correspond to the **case names** reported in the paper.

---

## JSON Structure

Each JSON file contains three main sections:

- `items`: part (piece) information  
- `plates`: board (bin) information  
- `parameters`: solver/runtime settings  

### `items` (parts)

Each element in `items` describes a part with the following fields:

- `BackFrontPriority`: whether the part is a priority part (`true`) or an ordinary part (`false`)
- `centPt`: center point of the part
- `id`: part ID
- `points`: polygon vertices of the part (coordinates)
- `smallItem`*: whether the part is considered small-sized

### `plates` (boards/bins)

Each element in `plates` describes a board type (bin type):

- `height`: board height
- `width`: board width
- `id`*: board ID (not used in the single-bin-size setting considered in the paper)
- `number`: number of available boards. In this work, boards are assumed to be unlimited, thus `number` is set to `9999`.
- `surplus`*: whether the board is a surplus sheet (reserved for future work)

### `parameters` (settings)

- `timeLimit`: time limit for the solver
- `remnantsSet`*: definition of remnants
- `surplusDir`*: whether to generate remnants during the computation

---

## Notes on Unused Fields

Fields marked with `*` are **not used** in the paper above. They are included for compatibility with an extended version of the dataset and will be utilized in future research.
