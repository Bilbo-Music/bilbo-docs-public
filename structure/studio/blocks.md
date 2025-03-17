# Basic Blocks

## Block:HeadButtons
- Main action buttons for the object.

## Block:Status
- Status switch for the object.

## Block:Menu
- Vertical menu.
- Manages the visibility of pages.

## Block:LoadMore
- "Load more" button if there is available content.

## Block:ResponsibleUser
- Representative of the object.
- Ability to change the representative by the curator.

---

# Users
## Block:PreviewUser
- On click: `block:User`

## Block:Users
- List of `PreviewUser` blocks.
- `block:LoadMore` (For users).

## Block:User
- `block:PreviewPlaylists` (Playlists where they are a representative).
- `block:PreviewArtists` (Artists where they are a representative).
- `block:HeadButtons` (Delete, Edit)
- Information about user roles.

---

# Artists
## Block:PreviewArtist
- On click: `block:Artist`

## Block:Artists
- List of `PreviewArtist` blocks.
- `block:LoadMore` (For artists).

## Block:Artist
- `block:Status`
- `block:PreviewTracks` (Tracks of the artist).
- `block:PreviewPlaylists` (Playlists of the artist).
- `block:ResponsibleUser`
- `block:HeadButtons` (Delete, Edit)
- Information about the artist:
  - Profile picture
  - Basic information
  - Artist genres

---

# Tracks
## Block:PreviewTrack
- Track image. On click: `block:Player.PlayTrack`.
- On click: `block:Track`

## Block:Tracks
- List of `PreviewTrack` blocks.
- `block:LoadMore` (For tracks).

## Block:Track
- `block:Status`
- `block:HeadButtons` (Delete, Edit, Upload files)

- `block:PreviewArtist` (Artist of the track).
- `block:ResponsibleUser`
- Information about the track:
  - Track image
  - Basic information
  - Rating, moods, tags
- Track files:
  - mp3
  - HD
  - Around
- Information about track licenses.

---

# Playlists
## Block:PreviewPlaylist
- On click: `block:Playlist`.

## Block:Playlists
- List of `PreviewPlaylist` blocks.
- `block:LoadMore` (For playlists).

## Block:Playlist
- `block:Status`
- `block:PreviewTracks` (Tracks of the playlist).
- `block:PreviewArtist` (Artist of the playlist).
- `block:ResponsibleUser`
- `block:HeadButtons` (Delete, Edit)
- Information about the playlist:
  - Playlist image
  - Basic information
  - Artist genres.

---

# Dictionaries
## Block:PreviewDictionary
- A dictionary is akin to a playlist collected on a specific theme.
- On click: `block:Dictionary`.

## Block:Dictionaries
- List of `PreviewDictionary` blocks.
- `block:LoadMore` (For dictionaries).

## Block:Dictionary
- `block:HeadButtons` (Delete, Edit)
- Information about the dictionary entry:
  - Dictionary entry image
  - Basic information

---

# Player
## Block:Player
- Open by default. A narrow bar pinned to the bottom left of the screen.
- Displays the current track: cover, title, author.
- Control buttons: next track, previous track, play, pause.
- Track rewind bar.

## Block:Player.PlayTrack
- Opens `block:Player`.
- Plays the track.
