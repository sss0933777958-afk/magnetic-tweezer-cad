# magnetic-tweezer-cad

Hexapole magnetic tweezer CAD model repository.

## Designs

### `hung/` — Hung Hexapole Design

6-pole magnetic tweezers with tilted poles on a R=0.5mm sphere at magic angle (54.74°).

| Folder | Contents |
|--------|----------|
| `step_for_fem/` | STEP files for FEM simulation (simplified, holes removed) |
| `reference/` | Reference materials (drawings, datasheets) |

#### Parts in `step_for_fem/`

| File | Description | Key Dimensions |
|------|-------------|---------------|
| `Mag_Pole_Bottom.STEP` | Magnetic pole (D-shape + cone) | R=3.175mm, total=43mm |
| `pole_upper_block.STEP` | Upper block (L-shape) | 25x22x10mm |
| `pole_lower_block.STEP` | Lower block (L-shape) | 22x22x10mm |
| `Mag_Guide_Post.STEP` | Guide post cylinder | R=4mm, H=46mm |
| `Coil.STEP` | Excitation coil | R_in=10, R_out=12, H=15mm |
| `Upper_Ring.STEP` | Yoke (iron ring) | R_in=38, R_out=62.5, T=2mm |
| `Full_Assembly_inch.STEP` | Complete assembly | All parts, inch units |

### `long-fei/` — Reference Design (Fei Long 2016)

Reference hexapole from Fei Long's PhD dissertation (Ohio State University, 2016).

| Folder | Contents |
|--------|----------|
| `step_for_fem/` | ANSYS-ready model (`MTmodel.step`) |
| `reference/` | APDL modeling scripts |

## Related Repository

FEM simulation scripts, MATLAB analysis, and results:
[magnetic-tweezers-sim](https://github.com/kevinfan100/magnetic-tweezers-sim)

## Reference

> Fei Long, "Active Control of the Probe-Sample Interaction Force at the Piconewton Scale by a Magnetic Microprobe in Aqueous Solutions," PhD dissertation, Ohio State University, 2016.
