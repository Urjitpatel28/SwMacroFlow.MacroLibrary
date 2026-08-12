# Change Document Unit

Sets the document's unit system and the individual length, angle, mass, volume, time, force, power
and energy units. Optionally switches inch dimensions to fractions.

**Runs per file**, on parts, assemblies and drawings.

## Inputs

| Field | Purpose |
|---|---|
| UnitSystem | `MMGS`, `IPS`, `MKS`, `CGS` or `Custom`. |
| LengthUnit | Length unit for the document. |
| DualLengthUnit | Length unit for dual dimensions. |
| AngleUnit | `degrees`, `deg/min`, `deg/min/sec` or `radians`. |

### Only read when UnitSystem is `Custom`

| Field | Purpose |
|---|---|
| CustomLength / CustomMass / CustomVolume | Custom system base units. |
| CustomTime / CustomForce / CustomPower / CustomEnergy | The rest of the custom system. |

### Fractions — only apply to IPS, or a Custom system using inches

| Field | Purpose |
|---|---|
| UseFractions | Show inch dimensions as fractions. |
| Denominator | Smallest fraction to show: 2, 4, 8, 16, 32 or 64. |
| RoundFractions | Round to the nearest fraction rather than showing a remainder. |

## Results

Reports the unit system and length unit that were applied, or the first unit name it could not
recognise.
