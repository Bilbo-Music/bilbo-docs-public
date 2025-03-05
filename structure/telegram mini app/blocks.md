
# Basic Blocks

## Block: Menu
- A horizontal menu that supports navigation through clicks and screen swipes.
- Manages the visibility of blocks.

## Block: LoadMore
- "Load More" button, if additional content is available.
- Activates automatically when fully visible on the screen.

## Block: Favorite
- Add to favorites / Remove from favorites.

---

# Artists

## Block: PreviewArtist
- Artist image. On click: `block:Player.PlayArtist`.
- Artist name. On click: `page:Artist`.
- Kebab menu. On click: `block:KebabArtist`.

## Block: PreviewArtists
- List of 8 `PreviewArtist` blocks arranged horizontally in one column with swipe capability.
- Button to navigate to `page:Artists`.

## Block: Artists
- List of `PreviewArtist` blocks.
- `block:LoadMore` (For artists).

## Block: DetailArtist
- Author information:
  - Name
  - Profile image
  - Description
  - Option to obtain email for commercial inquiries.
- Play button. On click: `block:Player.PlayArtists`.
- Kebab menu. On click: `block:KebabArtist`.
- `block:Favorite` (For the artist).
- `block:PreviewTracks` (Popular tracks).
- `block:PreviewPlaylists` (Artist's playlists).
- Links to official social media pages.

---

# Track

## Block: PreviewTrack
- Track image, title, author. On click: `block:Player.PlayTrack`.
- Kebab menu. On click: `block:KebabTrack`.

## Block: PreviewTracks
- List of 12 `PreviewTrack` blocks arranged horizontally with swipe capability (3 per row).
- Button to navigate to `page:Tracks`.

## Block: Tracks
- List of `PreviewTrack` blocks.
- `block:LoadMore` (For tracks).

---

# Playlist

## Block: PreviewPlaylist
- Playlist image. On click: `block:Player.PlayPlaylist`.
- Title and author of the playlist. On click: `page:Playlist`.
- Kebab menu. On click: `block:KebabPlaylist`.

## Block: PreviewPlaylists
- List of 12 `PreviewPlaylist` blocks arranged horizontally with swipe capability (1 per row).
- Button to navigate to `page:Playlists`.

## Block: Playlists
- List of `PreviewPlaylist` blocks.
- `block:LoadMore` (For playlists).

## Block: DetailPlaylist
- Playlist information:
  - Title
  - Playlist image
  - Duration
  - Number of tracks.
- Play button. On click: `block:Player.PlayPlaylist`.
- Kebab menu. On click: `block:KebabPlaylist`.
- Shuffle button: randomizes track order and starts playback.
- `block:PreviewArtist` (Author of the playlist).
- `block:Favorite` (For the playlist).
- `block:Tracks` (Tracks in the playlist).

---

# Dictionaries

## Block: PreviewDictionary
- A dictionary is similar to a playlist, compiled around a specific theme.
- Dictionary image. On click: `block:Player.PlayPlaylist`.
- Title. On click: `page:Playlist`.
- Kebab menu. On click: `block:KebabDictionary`.

## Block: PreviewDictionaries
- List of 12 `PreviewDictionary` blocks arranged horizontally with swipe capability (1 per row).
- Button to navigate to `page:Dictionaries`.

## Block: Dictionaries
- List of `PreviewDictionary` blocks.
- `block:LoadMore` (For dictionaries).

## Block: DetailDictionary
- Dictionary information:
  - Title
  - Dictionary image.
- Play button. On click: `block:Player.PlayPlaylist`.
- Kebab menu. On click: `block:KebabDictionary`.
- Shuffle button: randomizes track order and starts playback.
- `block:Tracks` (Tracks in the dictionary).

---

# Kebab Menus

## Block: KebabArtist
- Copy link.
- Share.
- `block:Favorite` (For the artist).

## Block: KebabTrack
- Download.
- Copy link.
- Share.
- Go to musician: `page.Artist`.
- Listen next (queue after the current track).
- Add to queue.
- Listen to similar.
- `block:Favorite` (For the track).
  
 If the user has the role of "**Playlist Curator**":
 - Add to playlist.

## Block: KebabPlaylist
- Listen next (queue after the current track).
- Share.
- Copy link.
- `block:Favorite` (For the playlist).

 If the user has the role of "**Playlist Curator**":
 - Edit playlist (only for playlist owner).

## Block: KebabDictionary
- Listen next (queue after the current track).
- Share.
- Copy link.

---

# Player

## Block: Player
- A player with two modes: Preview and Full.

### Preview mode
- Open by default. A narrow bar pinned to the bottom of the screen.
- Displays the current track: cover, title, author.
- `block:Favorite` (For the track).
- Control buttons: next track, previous track, play, pause.
- Track seek bar.
- Swipe up opens Full mode.

### Full mode
- Contains all Preview elements, plus:
- Kebab menu. On click: `block:KebabTrack`.
- Snippet mode toggle.
- Track quality toggle: normal, HD, around.
- Buttons: download, share, sleep timer, listen to similar, queue, shuffle.
- Toggles: repeat one song, repeat playlist, no repeat.

 If the user has the role of "**Playlist Curator**":
 - Button to add to playlist.

## Block: Player.PlayArtist
- Opens `block:Player` in Preview mode.
- Plays a playlist created from the artist's tracks.

## Block: Player.PlayTrack
- Opens `block:Player` in Preview mode.
- Plays a track.

## Block: Player.PlayPlaylist
- Opens `block:Player` in Preview mode.
- Plays a playlist.
