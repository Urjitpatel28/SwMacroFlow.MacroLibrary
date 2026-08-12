# Save with Performance Improvement

Turns image quality down to its cheapest settings — shaded deviation at maximum, high-quality edges
off, wireframe quality at its lowest — then saves a copy named `<name>_Optimized`.

The original file is left alone; only the copy carries the reduced settings.

**Runs per file**, on parts, assemblies and drawings.

## Inputs

| Field | Purpose |
|---|---|
| SaveModelData | Drawings only: keep model data in the saved file. Off makes the drawing much smaller but it can no longer be opened without its model. |
| SavePath | Where to save. Blank saves beside the original. |
| SubFolder | Put the saved file in an `\Optimized` subfolder, created if missing. |

## Results

Reports the path it wrote, or "Invalid Save path" if `SaveAs` was refused.
