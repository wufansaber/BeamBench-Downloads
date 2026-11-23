# Optical component library

Open **Insert component** or expand a family on the left of an optical bench. **Browse supplier parts** opens that family in the catalog. Search by Thorlabs or Edmund Optics stock number. The **Traceable optics** filter selects models the BeamBench ray tracer can run. **Original optical files** selects products with a manufacturer design file.

| Model shown in the catalog | What BeamBench uses |
| --- | --- |
| Manufacturer website prescription | Optical surfaces and materials read from a supplier product download. Expand **Original optical models** to choose a particular supported file. |
| Manufacturer stock prescription | Optical geometry from a manufacturer stock design in the OpticStudio lens catalog. |
| Datasheet-derived model | Geometry and optical response reconstructed from published parameters. The detail pane states which effects are included. |
| Native design file | The original design can be downloaded or attached to a project. An unsupported surface, archive or Code V sequence may need its originating solver. |
| Parameters required | Enter a prescription through **Define from parameters…**. The form identifies its starting values as an editable template. |

**Insert in bench** places an independent component at a 3D position. A wavelength-dependent part can be placed before choosing the operating wavelength. The inspector identifies the specified band or design wavelength. When a model requires the geometric optical bench, **Create optical bench with this part** creates another project and preserves the current project in the browser project library.

**Custom / import .bbpart…** opens a parameter form. Select the optical model, enter its dimensions and interaction parameters, and click **Insert in bench**. **Save .bbpart** exports a reusable part. Open the same form and choose the file under **Import parameters** to reuse it. **File → Save project** stores inserted components and attached originals in the project’s `.bbproj`. An attached original appears under **Original model files** in the optical path pane.

For Edmund Optics **14-689**, use **Beamsplitters**, insert the part, place a collimated source and a sufficiently large power detector, and select **1064 nm**. The model distributes 82% of incident power across six intended output orders with nominally equal weights. The angular separation is 0.76°. Spot-to-spot nonuniformity, interference and residual orders require additional data. A cube has two outgoing ports and its nominal R/T ratio sets their weights.

The insertion library covers functional optics, sources and light detectors. Mounted optical components retain their stock identity. Empty supports and adapters are screened out. A mechanical STEP drawing alone does not supply an optical prescription.
