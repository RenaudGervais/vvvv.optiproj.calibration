# vvvv.optiproj.calibration
Manual calibration between an optitrack target and a projector

The idea is to speed up the process by entering model-space points once and then only entering projection space in batches.

## Entering model points
Start `SetModelPoints` patch and check for documentation on keyboard command inside the patch.

## Calibrating the projector
Start `CalibrateProjector` patch and check for documentation on inside the patch. Basically, it will load up the points you saved in the previous process and apply the OptiTrack transform to it. You have to select the points in projection space according to the currently highlighted point. Cycle through the model points with PgUp/PgDown keys. Press space to enqueue the current set of points.

When satisfied with the calibration, scroll down the patch and write the calibration to file.