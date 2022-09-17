# Desktop Parser

This is a parser for the [`.desktop` file format](https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html). It's used in [Desktop Creator](https://github.com/DesktopCreatorTeam/DesktopCreator).

## Installation

### From pypi

```bash
pip install desktop-parser
```

### From source

```bash
git clone https://github.com/DesktopCreatorTeam/desktop-parser
cd desktop-parser
poetry install
```

### From the AUR

```bash
yay -S python-desktop-parser
```

## Usage

```python
from desktop_parser import DesktopFile

# Parse a file
desktop_file = DesktopFile.from_file("path/to/file.desktop")

desktop_file.data["Name"] = "New Name"
desktop_file.data["Exec"] = "new-exec"

# Save the file
desktop_file.save("path/to/file.desktop")
```

## Documentation

The documentation is available [here](https://desktopcreatorteam.github.io/desktop-parser/).

## License

This project is licensed under the GNU GPLv3 license - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

* [Desktop Entry Specification](https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html)

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors and Contributors

* [Desktop Creator Team](https://github.com/DesktopCreatorTeam/DesktopCreator)
    - **[0xMRTT](https://github.com/0xMRTT)**