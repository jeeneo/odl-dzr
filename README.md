# odl-dzr
[OrpheusDL](https://github.com/OrfiTeam/OrpheusDL) module for downloading music from [Deezer](https://www.deezer.com/)

## This fork:
1. Adds `genre` and `album_artist` tags
2. Adds support for `dzr.page.link` when downloading

## Getting started
### Prerequisites
- [OrpheusDL](https://github.com/OrfiTeam/OrpheusDL), duh

### Installation
- Clone the repository in your `orpheusdl` (root) directory:
```
git clone https://github.com/jeeneo/odl-dzr modules/deezer
```
- Update `config/settings.json` with Deezer settings:
- `python orpheus.py`

## Configuration

<details>
<summary>Global</summary>

`download_quality`:
| Value      | Format              |
| ---------- | ------------------- |
| "hifi"     | 16-bit 44.1kHz FLAC |
| "lossless" | 16-bit 44.1kHz FLAC |
| "high"     | MP3 320kbps         |
| "medium"   | MP3 320kbps         |
| "low"      | MP3 128kbps         |
| "minimum"  | MP3 128kbps         |

`main_resolution`:
Maxes out at 3000px  
If original cover size is smaller than the one specified, falls back to 1200px

</details>

<details>
<summary>Deezer</summary>

| Setting         | Description                                         |
| --------------- | --------------------------------------------------- |
| `client_id`     | Client ID used for login                            |
| `client_secret` | Client secret used for login                        |
| `bf_secret`     | Constant for deriving key used for track decryption |
| `email`         | Account email                                       |
| `password`      | Account password                                    |

</details>


## Credits
<details>
<summary>Credits</summary>

[@uhwot](https://github.com/uhwot) for the module base

[@TheKVT](https://github.com/TheKVT) their edits (ARL support and misc fixes)
  
[@OrfiTeam](https://github.com/OrfiTeam) for OrpheusDL

</details>
