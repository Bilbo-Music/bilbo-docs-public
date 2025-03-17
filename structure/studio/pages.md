# Pages
## Page:Roles
- Contains `block:Dictionaries(roles)`.
- Contains `block:Dictionary(role)`.
- `block:HeadButtons` (Add role)

## Page:Category
- Contains `block:Dictionaries(categories)`.
- Contains `block:Dictionary(category)`.
- `block:HeadButtons` (Add category)

## Page:Genres
- Contains `block:Dictionaries(genres)`.
- Contains `block:Dictionary(genre)`.
- `block:HeadButtons` (Add genre)

## Page:Instruments
- Contains `block:Dictionaries(instruments)`.
- Contains `block:Dictionary(instrument)`.
- `block:HeadButtons` (Add instrument)

## Page:Moods
- Contains `block:Dictionaries(moods)`.
- Contains `block:Dictionary(mood)`.
- `block:HeadButtons` (Add mood)

## Page:Tags
- Contains `block:Dictionaries(tags)`.
- Contains `block:Dictionary(tag)`.
- `block:HeadButtons` (Add tag)

## Page:Users
- Contains `block:Users`.
- Contains `block:User`.

## Page:Playlists
- Contains `block:Playlists`.
- Contains `block:Playlist`.
- `block:HeadButtons` (Add playlist)

## Page:Artist
- Contains `block:Artists`.
- Contains `block:Artist`.
- `block:HeadButtons` (Add artist)

## Page:Track
- Contains `block:Tracks`.
- Contains `block:Track`.
- `block:HeadButtons` (Add track)

---

# Navigation
- The navigation menu is located on the left. It consists of a set of links to pages, each of which is accessible to users with a specific role:

>     [
>      	page:Roles { admin },
>      	page:Category { dictionary_curator },
>      	page:Genres { dictionary_curator },
>      	page:Instruments { dictionary_curator },
>      	page:Moods { dictionary_curator },
>      	page:Tags { dictionary_curator },
>      	page:Users { admin, playlist_curator, artist_curator },
>      	page:Playlists { all users },
>      	page:Artists { all users },
>      	page:Tracks { track_curator or if there are artists where the user is the representative },
>     ]
