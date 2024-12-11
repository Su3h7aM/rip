<div align="center">

# rip

### A modern replacement for `rm`

</div>

`rip` (Rm ImProved) is a modern replacement for the classic `rm` command, built in Go with a focus on safety, user-friendliness, and adherence to modern standards. Instead of permanently deleting files, `rip` moves them to the trash following the [XDG Trash Specification](https://freedesktop.org/wiki/Specifications/trash-spec/), making recovery simple and reliable.

### Goals

- **XDG Trash Compliance:** Ensures files and directories are recoverable by moving them to the user's trash.
- **Accident Prevention:** Provides a safer alternative to `rm` by avoiding immediate data loss.
- **Simple and Intuitive:** Retains a familiar interface while enhancing functionality.
- **Cross-Platform Support:** Works seamlessly on Linux and macOS.

### How to Use

`rip` works similarly to `rm`, but files are moved to the trash instead of being permanently deleted.

#### Basic Syntax

```sh
rip [OPTIONS] FILE...
```

#### Options

- `-r`, `--recursive`  Remove directories and their contents recursively.
- `-f`, `--force`      Suppress warnings and prompts.
- `-i`, `--interactive` Ask for confirmation before each removal.
- `--version`          Show the version information.
- `--help`             Display help text.

### Examples

```sh
# Move a file to the trash
rip example.txt

# Remove a directory recursively
rip -r my-folder

# Interactive deletion
rip -i file1.txt file2.txt
```

### Contributing

This project is a work in progress. If you want to contribute, feel free to open issues, submit pull requests, or discuss ideas for improving the project!
