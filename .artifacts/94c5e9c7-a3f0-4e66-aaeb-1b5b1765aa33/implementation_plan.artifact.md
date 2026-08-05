# Implementation Plan - Spotify Style SVG Icons

The user wants to change the play/pause, next, and previous icons to a Spotify-like SVG style. This involves replacing the current vector path data with simpler, more solid shapes that match Spotify's aesthetic (solid triangles and bars).

## Proposed Changes

### [Resources]

#### [MODIFY] [play.xml](file:///D:/flux%20copy/Metrolist-main/app/src/main/res/drawable/play.xml)
- Replace complex path data with a solid, slightly rounded triangle.

#### [MODIFY] [pause.xml](file:///D:/flux%20copy/Metrolist-main/app/src/main/res/drawable/pause.xml)
- Replace complex path data with two solid vertical bars.

#### [MODIFY] [skip_next.xml](file:///D:/flux%20copy/Metrolist-main/app/src/main/res/drawable/skip_next.xml)
- Replace complex path data with a solid triangle followed by a vertical bar.

#### [MODIFY] [skip_previous.xml](file:///D:/flux%20copy/Metrolist-main/app/src/main/res/drawable/skip_previous.xml)
- Replace complex path data with a vertical bar followed by a solid triangle.

## Verification Plan

### Manual Verification
1. Open the player screen.
2. Observe the Play/Pause, Next, and Previous icons.
3. Verify they look solid and follow the Spotify aesthetic.
4. Test playback controls to ensure icons toggle correctly (Play <-> Pause).
