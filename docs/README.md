# Scripts

`find_*_offsets.py` outputs pattern matched hacks to json

`json_to_bemanipatcher.py` autoruns with `find_*_offsets.py` 

Note:

- Patterns break, fix it yourself

- Append datecodes (ex. `game-2022123100.dll`) to do multiple DLLs at once

- Windows run all scripts: `for %s in (find*offsets.py) do python %s`

- Linux/Mac run all scripts: `for s in find*offsets.py; do python3 "$s"; done`

# Memory Patcher

`h4x0r.py` uses [pymem](https://github.com/srounet/Pymem) to toggle hacks in memory without modifying files on disk

Add hacks to whitelist (user friendly frontend soonTM)

Example: `python h4x0r.py --json game-2022123100.json --launcher bootstrap.exe --delay 0.65`
