---
name: ae-planar-studio
description: Prepare independent replaceable footage inserts for moving surfaces in Adobe After Effects and Mocha AE, and verify the tracked composite.
---

Inspect the live composition, frame duration, footage interpretation, layer transforms and existing inserts. Select one available AE bridge for inspection and edits. Use stable match names for multilingual installations. Record the identity of protected layers. Group reversible edits by panel.

For each physical surface choose a reference frame with four clear corners. Make a separate footage layer with its own Mocha AE instance and independent project data. In Mocha draw a spline around persistent coplanar detail, exclude foreground occluders, and track forward and backward from the reference. Enable perspective when supported by the image. Position the planar Surface on the inner rim. Scrub with the grid visible to distinguish tracking drift from a misplaced Surface. Trim to visible frames and check partially visible entry and exit. Reopen the saved Mocha project and verify the named layer, tracked range and animated surface before reporting a solve.

Export four corners to a dedicated precomp per insert. Map source pixel coordinates through the footage layer transform and into insert-layer coordinates at each sample time. Do not apply a translation twice. Keep only one active perspective deformation. To refine an entire track, map the corrected reference corners back to plane coordinates and reproject those coordinates at each frame. Use individual corrections if the grid itself drifts.

Inside each precomp keep one clearly named replacement layer. Fit footage to cover the canvas and adjust framing there. Verify with an asymmetric test image labelled at each corner. Inspect full-resolution renders at entry, reference, closest approach, strongest perspective, last partial frame and first frame after exit. Check all four edge strips for uncovered interior, clipped glow, and foreground occlusion. Report which frames were inspected. Stop at the requested batch size for review.

User handoff: open the numbered source precomp, select its placeholder and Alt-drag imported footage from Project onto that layer (Option-drag on macOS). Adjust Scale and Position inside the precomp. Preview the master composition. Changing the master insert's transform changes its alignment.
