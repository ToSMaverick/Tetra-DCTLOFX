# Tetra-DCTLOFX

The Tetra transformation, as described by Steve Yedlin ASC, originally implemented by for Nuke by calvinsilly, ported to Fusion by EmberLightVFX, and presented here as a DCTL for the ResolveFX DCTL plug-in.

## HSL Controls
This is a fork of npeason's versoin to provice HSL-like controls. This should make camera matching via the vectorscope way easier.

## Installation:

1. Find Your LUT folder by opening File>Project Settings. Select *Color Management*, then under *Lookup Tables*, click *Open LUT Folder*.
2. Put Tetra.dctl in there somewhere.
3. Restart Resolve.

## Usage:
1. Apply *DCTL* OFX from *ResolveFX Color* category to desired node.
2. Select the Tetra.dctl file from *DCTL List*

**Note:** Control parameters are "normalized" so they are zero at unity. But, for the algorithm, values must correspond to their actual position on the cube. eg: the Red-Red value must be 1.0 at unity, so 1.0 is added to the entered value.

## Credits:
1. calvinsilly's Nuke implementation: https://github.com/calvinsilly/Tetrahedral-Interpolation
2. EmberLightVFX's Fusion implementation: https://github.com/EmberLightVFX/Tetrahedral-Interpolation-for-Fusion
3. Yedlin's video hinting at this transform: http://www.yedlin.net/DisplayPrepDemo/DispPrepDemoFollowup.html
4. npeason's Resolve implementation: https://github.com/npeason/Tetra-DCTLOFX
