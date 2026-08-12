# Save PDF

Exports the open document to PDF. Works on parts, assemblies and drawings.

**Runs per file** — point the scope at a folder and it exports each document in turn.

## Inputs

| Field | Purpose |
|---|---|
| OutputName | PDF file name, without the `.pdf` extension. Required. |
| OutputFolder | Where the PDF goes. Blank saves it beside the document. Created if missing. |
| Options | Free text matched against the option names below. Combine as many as you like. |
| SheetName | Drawings only. A sheet name, or a comma-separated list. Blank exports every sheet. |

### Options

| Word | Effect |
|---|---|
| `Zoom Model` | Zoom to fit before exporting. |
| `Open Created PDF` | Open each PDF in the default viewer. **Leave this out of an unattended batch** — it opens a window per file. |
| `Save Only Current Sheet` | Drawings: export just the active sheet. Ignored if SheetName is set. |
| `Save 3D PDF` | Parts and assemblies: export as a 3D PDF. |

## Results

Reports the path it wrote, or the SOLIDWORKS error code if `SaveAs` failed.
