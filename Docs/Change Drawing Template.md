# Change Drawing Template

Applies a `.slddrt` sheet format to one sheet, several named sheets, or every sheet in a drawing,
then rebuilds and saves.

**Runs per file**, on drawings. Parts and assemblies are reported as unsupported.

## Inputs

| Field | Purpose |
|---|---|
| SheetName | A sheet name, or a comma-separated list. Blank means every sheet. |
| TemplatePath | The `.slddrt` sheet format to apply. |

`SheetName` examples: `""` for all sheets, `Sheet1` for one, `Sheet1, Sheet2` for several.

## Results

Reports how many sheets were updated. A file where **no** sheet could be updated is reported as an
error; a partial update is reported with the last error in the message.
