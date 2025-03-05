# Pages

## Page: Tracks
- Contains `block:Tracks`.

## Page: Playlist
- Contains `block:DetailPlaylist`.

## Page: Playlists
- Contains `block:Playlists`.

## Page: Dictionary
- Contains `block:Dictionary`.

## Page: Dictionaries
- Contains `block:DetailDictionary`.

## Page: Artist
- Contains `block:DetailArtist`.

## Page: Favorite
- Contains `block:Menu` (Tracks, Playlists, Artists), as well as:
  - `block:Tracks` (favorite tracks).
  - `block:Playlists` (favorite playlists).
  - `block:Artists` (favorite artists).

## Page: Profile
- Current user page.
- Settings:
  - Theme customization (options: Telegram style, light, dark).
  - Language translation settings (default as in Telegram, choice from available languages).
  - Option to connect Tonkeeper.
  - Option to change name.
  - Option to change profile image.
  - Notification settings.
  - Enable/disable vibration.
  - Authorization option in **Studio**.

## Page: Search
- Input field for search.
- Contains `block:Menu` (Tracks, Playlists, Artists), as well as:
  - `block:Tracks` (found tracks).
  - `block:Playlists` (found playlists).
  - `block:Artists` (found artists).

## Page: Music
- Contains:
  - `block:PreviewPlaylist` (Premiere, best new tracks).
  - `block:PreviewPlaylists` (Curated by editors).
  - `block:PreviewDictionaries` (Categories, Genres, Moods).
  - `block:PreviewArtists` (New artists).

  If the user is **an artist representative**:
  - `block:PreviewArtists` (Artists).

  If the user has the role of "**Playlist Curator**":
  - `block:PreviewPlaylists` (Playlists created by them).


## Page: Aura
- Description will come after MVP (1).

## Page: Royality
- Description will come after MVP (2).

## Page: Hexa
- Description will come after MVP (3).

---

# Navigation
- The navigation menu is located at the bottom. It consists of a set of small carousels, which can be switched by swiping up and down, as well as by clicking the same button again:

>     [ 
>         [page:Music, page:Favorite, page:Hexa],
>         [page:Aura],
>         [page:Search],
>         [page:Royality],
>         [page:Settings]
>     ]

- On each page, except for those in the above array, there is an option to go back using the "Back" button in the upper left corner or by swiping, unless overridden by another block.
