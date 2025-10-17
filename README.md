# bfbbps2

This repository does **not** contain any game assets or assembly whatsoever. An existing copy of the game is required.

# Dependencies

## Windows

On Windows, it's **highly recommended** to use native tooling. WSL or msys2 are **not** required.  
When running under WSL, [objdiff](#diffing) is unable to get filesystem notifications for automatic rebuilds.

- Install [Python](https://www.python.org/downloads/) and add it to `%PATH%`.
  - Also available from the [Windows Store](https://apps.microsoft.com/store/detail/python-311/9NRWMJP3717K).
- Install Splat
  - Quick install via pip: `python3 -m pip install -U splat64[mips]`

  # Splitting

- Clone the repository:

  ```sh
  git clone https://github.com/bfbbdecomp/bfbb.git
  ```

- Put `SLUS_206.80` in the iso folder

- run `python3 -m splat split config/bfbb.yaml`
