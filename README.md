# HVAC Leak-Rate Practice Helper (Educational)

Python **stdlib-only** CLI to practice annualized leak-rate math and compare against **educational** category threshold presets.

> **NOT a compliance system / NOT legal advice.**  
> Real AIM Act / Section 608 audits need dedicated tools (608Log-class) and current regulatory text.

## Quick start

```bash
cd hvac-leak-rate-helper
python3 leak_rate_helper.py --help
python3 leak_rate_helper.py -i
```

### Example

```bash
python3 leak_rate_helper.py \
  --full-charge-lbs 50 \
  --added-lbs 8 \
  --days 90 \
  --category commercial-refrigeration \
  --chem hfc
```

## Categories

`comfort-cooling` · `commercial-refrigeration` · `industrial` · `transport`

Annualized % ≈ `(added / full_charge) × (365 / days) × 100`
