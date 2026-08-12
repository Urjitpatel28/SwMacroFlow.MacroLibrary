# Insert Block In Drawings

Inserts a `.sldblk` sketch block at a fixed position on one sheet, several named sheets, or every
sheet in a drawing, then rebuilds and saves.

**Runs per file**, on drawings.

## Inputs

| Field | Purpose |
|---|---|
| BlockPath | The sketch block file to insert. |
| XPosition | X position on the sheet, in mm from the sheet origin. |
| YPosition | Y position on the sheet, in mm from the sheet origin. |
| Angle | Rotation in degrees. |
| Scale | Scale factor; `1` is full size. |
| SheetName | A sheet name, or a comma-separated list. Blank means every sheet. |

The four numeric fields are plain text boxes because everything reaches a macro as a string; leave
one blank and it falls back to its neutral value (0, or 1 for Scale).

## Results

Reports how many sheets the block was inserted on.
