Seamless Hemp House — Open-Source Blueprint & Precision Hardware Specification (V2)


An open-source, precision-indexed modular building system uniting Hemp OSB, HempWool insulation, high-pressure pressed aluminum-sandwiched hemp trusses, locking saddles, recessed hemp-stud twist-key locks, press-lock-and-seal openings, Hemp Nano-Carbon Crete, pre-installed nano-copper-lined PEX, and targeted exterior polyurethane sealing over a vapor-open rainscreen.


License & Open-Source Terms
This blueprint, bill of materials, manufacturing specification, hardware tolerance schedule, utility integration notes, and parametric scaling scripts are released under the Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).

Share: Copy and redistribute the material in any medium or format for commercial, residential, or individual/owner-builder use.
Adapt: Remix, transform, and build upon the material for any purpose.
Attribution: Give appropriate credit, provide a link to the license, and indicate if changes were made.
ShareAlike: If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

Full legal text: https://creativecommons.org/licenses/by-sa/4.0/legalcode

Engineering, Health & Code Notice: Structural spans, truss engineering, uplift/shear saddle capacities, slab/nano-carbon-crete structural design, potable/thermal nano-copper PEX suitability, particulate/worker safety controls, fire/egress codes, and regional wind, snow, or seismic requirements must be verified with a licensed structural/plumbing engineer and local Authority Having Jurisdiction (AHJ) prior to fabrication or construction.


Core System Architecture
Baseline & Larger-Scale Footprints: Starts from a 24 ft × 44 ft (1,056 sq ft) baseline and scales linearly in 2 ft (24 in), 4 ft (48 in), and 8 ft (96 in) increments—including 8 ft × 8 ft modular runs extending past 100 ft and larger footprints such as 32 ft × 64 ft, 44 ft × 100 ft, 48 ft × 104 ft, and 64 ft × 120 ft.
Modular Grids & Roof Datum: Aligned to 16 in O.C. and 24 in O.C. framing/saddle stations, 4 ft (48 in) coincidence checkpoints and truss spacing, and a 2 ft (24 in) walls-to-peak datum.
Hemp OSB (4'×8' and 6'×12'): Grade S1 (7/16 in exterior wall and roof sheathing), Grade S2 (3/4 in T&G subfloor), and Grade I1 (1/2 in smooth interior board), pressed with a 3-stage degas cycle.
Insulation & Composite Trusses: HempWool R-20 batts (walls/floor) and HempWool R-13 batts (double-layer ceiling), paired with high-pressure pressed aluminum-sandwiched hemp trusses locked into mechanical saddles.
Hemp Nano-Carbon Crete & Pre-Installed Nano-Copper PEX: Integrates hemp-reinforced nano-carbon crete slab/base/composite elements with nano-copper-lined PEX pre-routed or pre-installed in crete and wall chases prior to finish close-in.
Locks, Openings & Vapor-Open Envelope: Recessed hemp-stud twist-key locks engaging headers and side studs, press-lock-and-seal doors and windows, and targeted exterior polyurethane sealant at expansion joints, saddles, and opening perimeters over a vapor-open rainscreen wall assembly.


Exact 1/16 in Precision Schedule (Framing, Locks & Pre-Installed PEX)
Dimension / Tolerance
Standard
Exact 1/16 in
Field & Fit Notes
16 in O.C. Grid
16 in
256/16 in
3 spaces per 48 in (4 ft)
24 in O.C. Grid
24 in
384/16 in
2 spaces per 48 in (4 ft)
2 ft Walls-to-Peak Datum
24 in
384/16 in
±1/16 in datum tolerance
4 ft Truss / Coincidence Mark
48 in
768/16 in
Coincidence line for 16 in & 24 in grids
8 ft Module Increment
96 in
1536/16 in
Linear module (13 × 8 ft = 104 ft / 19968/16 in)
Single 2× Stud / Plate
1 1/2 in
24/16 in
Nominal framing thickness (±1/16 in)
Double 2× Header / Jamb
3 in
48/16 in
Structural anchor zone for deep strike pockets
Hemp Stud Lock Recess
7/8 in
14/16 in
Leaves 5/8 in (10/16 in) rear wall in 1 1/2 in stud
Bolt / Latch Throw
3/4 in - 7/8 in
12/16 in - 14/16 in
Positive engagement into header/stud/jamb receiver
Pocket Bottom-Out Clearance
1/8 in - 3/8 in
2/16 in - 6/16 in
Prevents bottom-out binding
Compression Cam Pull
1/16 in - 3/16 in
1/16 in - 3/16 in
Draws sash/door into perimeter compression gasket
1/2" PEX CTS / Chase Sleeve
5/8 in OD / 3/4 in sleeve
10/16 in OD / 12/16 in sleeve
1/8 in (2/16 in) movement clearance (±1/16 in alignment)
3/4" PEX CTS / Chase Sleeve
7/8 in OD / 1 in sleeve
14/16 in OD / 16/16 in sleeve
1/8 in (2/16 in) movement clearance (±1/16 in alignment)
1" PEX CTS / Chase Sleeve
1 1/8 in OD / 1 1/4 in sleeve
18/16 in OD / 20/16 in sleeve
1/8 in (2/16 in) movement clearance (±1/16 in alignment)
Roof Sheathing Expansion Gap
1/8 in
2/16 in
Sealed with exterior polyurethane before finish roofing
Flush & Alignment Tolerance
±1/16 in
±1/16 in
Hardware, chase & grid verification tolerance



Hemp Nano-Carbon Crete & Pre-Installed Nano-Copper PEX Rules
Pre-Installation & Pressure Testing: Route and sleeve nano-copper-lined PEX in crete and wall chases before final casting or wall-board closure, then pressure-test and inspect all runs and stub-ups prior to concealment.
Thermal & Mechanical Isolation: Provide smooth sleeves, grommets, and 1/8 in (2/16 in) movement clearance at crete/stud transitions so thermal cycling and nano-carbon-crete cure/shrinkage do not abrade or bind PEX lines.
Vapor-Open Envelope Integrity: Preserve the vapor-open rainscreen wall stack and apply exterior polyurethane sealant strictly at targeted expansion joints (1/8 in / 2/16 in), roof/saddle penetrations, and opening perimeters rather than trapping moisture inside walls.


General Contractor (GC) Accountability
Across commercial, residential, and individual/owner-builder projects, responsibility for field execution, jobsite layout verification, hardware mortising and locking, hemp nano-carbon-crete placement, pre-installed nano-copper PEX testing/sleeving, targeted polyurethane sealing, vapor-open rainscreen detailing, and local building/plumbing code or structural engineering compliance rests with the General Contractor (GC).


Parametric Footprint Scaler (scale_blueprint.py)
from fractions import Fraction


def to_sixteenths_str(inches: float) -> str:
    sixteenths = round(inches * 16)
    frac = Fraction(sixteenths, 16)
    whole = int(frac)
    rem = frac - whole
    if whole == 0 and rem == 0:
        return '0" (0/16")'
    if whole == 0:
        return f'{rem.numerator}/{rem.denominator}" ({sixteenths}/16")'
    if rem == 0:
        return f'{whole}" ({sixteenths}/16")'
    return f'{whole} {rem.numerator}/{rem.denominator}" ({sixteenths}/16")'


def calculate_scale(width_ft: float, length_ft: float, lock_sets: int = 20) -> dict:
    area_sqft = width_ft * length_ft
    w_in = int(round(width_ft * 12))
    l_in = int(round(length_ft * 12))
    trusses_24 = (l_in // 24) + 1
    saddles_24 = trusses_24 * 2
    saddles_16_2walls = ((l_in // 16) + 1) * 2
    trusses_48 = (l_in // 48) + 1
    saddles_48 = trusses_48 * 2
    mat_freight_scaled = round(14434.80 * (area_sqft / 1056.0), 2)
    est_total = round(mat_freight_scaled + (saddles_24 * 14.00) + (lock_sets * 28.50), 2)
    return {
        "footprint": f"{width_ft:g} ft x {length_ft:g} ft",
        "area_sqft": area_sqft,
        "width_exact": to_sixteenths_str(w_in),
        "length_exact": to_sixteenths_str(l_in),
        "saddles_16_2walls": saddles_16_2walls,
        "trusses_24": trusses_24,
        "saddles_24": saddles_24,
        "trusses_48": trusses_48,
        "saddles_48": saddles_48,
        "lock_sets": lock_sets,
        "est_total_usd": est_total,
    }


if __name__ == "__main__":
    for dims, locks in [((8, 104), 16), ((24, 44), 20), ((44, 100), 83)]:
        print(calculate_scale(dims[0], dims[1], lock_sets=locks))

# full-hemp-house-locking-roof-doors-windos-Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).Seamless Hemp House — Open-Source Blueprint & Precision Hardware Specification
​An open-source, precision-indexed modular building system designed around Hemp OSB, HempWool insulation, high-pressure pressed aluminum-sandwiched hemp trusses, locking saddles, recessed hemp-stud twist-key locks, press-lock-and-seal openings, and targeted exterior polyurethane sealing over a vapor-open rainscreen.
​License & Open-Source Terms
​This repository and its blueprints, bills of materials, field tolerances, and parametric scaling scripts are released under the Creative Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0).
​Share: Copy and redistribute the material in any medium or format, for commercial, residential, or individual/owner-builder use.
​Adapt: Remix, transform, and build upon the material for any purpose.
​Attribution: Give appropriate credit, provide a link to the license, and indicate if changes were made.
​ShareAlike: If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.
​Full legal text: https://creativecommons.org/licenses/by-sa/4.0/legalcode
​Engineering & Code Notice: Structural spans, truss engineering, uplift/shear saddle capacities, fire/egress codes, and regional wind, snow, or seismic requirements must be verified with a licensed structural engineer and local Authority Having Jurisdiction (AHJ) prior to fabrication or construction.
​Core System Architecture
​Baseline Footprint: 24\text{ ft} \times 44\text{ ft} (1,056\text{ sq ft}), scalable linearly in 2\text{ ft} (24\text{ in}), 4\text{ ft} (48\text{ in}), and 8\text{ ft} (96\text{ in}) increments, including 8\text{ ft} \times 8\text{ ft} modules expanding past 100\text{ ft} and larger footprints such as 44\text{ ft} \times 100\text{ ft}.
​Modular Grids & Geometry: Aligned to 16\text{ in O.C.} and 24\text{ in O.C.} framing/saddle stations, 4\text{ ft} (48\text{ in}) coincidence checkpoints and truss spacing, and a 2\text{ ft} (24\text{ in}) walls-to-peak datum.
​Materials:
​Hemp OSB (4'×8' and 6'×12'): Grade S1 (7/16\text{ in} exterior wall & roof sheathing), Grade S2 (3/4\text{ in} T&G subfloor), and Grade I1 (1/2\text{ in} smooth interior board), pressed with a 3-stage degas cycle.
​Insulation: HempWool R-20 batts (walls/floor) and HempWool R-13 batts (double-layer ceiling).
​Composite Trusses & Saddles: High-pressure pressed aluminum-sandwiched hemp trusses locked into mechanical saddles.
​Locks & Openings: Recessed hemp-stud twist-key locks engaging headers and side studs, paired with press-lock-and-seal doors and windows.
​Weather & Vapor Control: Targeted moisture-curing exterior polyurethane sealant at roof sheathing expansion joints, truss saddles, strike collars, and opening perimeters while preserving a vapor-open rainscreen wall stack.
​Exact 1/16\text{ in} Precision Schedule