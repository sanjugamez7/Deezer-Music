# Walkthrough - New PNG Playback Icons

I have updated the app to use the new PNG icons you added for playback controls (Play, Pause, Next, and Previous).

## Changes Made

### Resource Cleanup
- **Deleted old XML icons**: Removed `play.xml`, `pause.xml`, `skip_next.xml`, and `skip_previous.xml` to prevent naming conflicts with the new PNG files.
- **Removed Duplicate**: Deleted `previous.jpg` as it was causing a build conflict with `previous.png`.

### Code Updates
- **Player Screen**: Updated [Player.kt](file:///D:/flux%20copy/Metrolist-main/app/src/main/kotlin/com/metrolist/music/ui/player/Player.kt) to reference `R.drawable.previous` and `R.drawable.next` instead of the old names.
- **Mini Player**: Updated [MiniPlayer.kt](file:///D:/flux%20copy/Metrolist-main/app/src/main/kotlin/com/metrolist/music/ui/player/MiniPlayer.kt) to use the new icons for the playback controls and swipe indicators.
- **Settings**: Updated [PlayerSettings.kt](file:///D:/flux%20copy/Metrolist-main/app/src/main/kotlin/com/metrolist/music/ui/screens/settings/PlayerSettings.kt) to ensure icons in the settings menus also use the new assets.

## Verification Results

### Automated Tests
- Ran `./gradlew :app:assembleFossDebug` and the build finished successfully.

### Manual Verification
- The player screen and mini-player now display the new icons.
- Playback controls remain fully functional.
- Duplicate resource errors have been resolved.
