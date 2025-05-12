# build-your-git

A simple, minimal Git implementation in Python based on the concepts from "The Stupid Content Tracker". This tool demonstrates the core mechanics of Git: object storage, commits, trees, branches, tags, and more—without external dependencies.

## Features

- Initialize a new repository (`init`)
- Add files to the index (`add`)
- Remove files (`rm`)
- Create commits with messages (`commit`)
- Inspect objects (`cat-file`, `hash-object`)
- List directory trees (`ls-tree`)
- List files in the index (`ls-files`)
- Show commit history graph (`log`)
- Show and parse references (`show-ref`, `rev-parse`)
- Create and list tags (`tag`)
- Check ignore patterns (`check-ignore`)
- Show working tree status (`status`)
- Checkout trees or commits into a directory (`checkout`)

## Prerequisites

- Python 3.7 or newer
- Standard library modules only (no external dependencies)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/kdjayyyy/build-your-git.git
   ```

2. Change to the project directory:
   ```bash
   cd build-your-git
   ```

3. Ensure `libwyag.py` is executable or invoke with Python:
   ```bash
   python libwyag.py <command> [options]
   ```

## Usage

After cloning or downloading the project, you can use it via the command line in a Unix-like environment (Linux, macOS, or Windows with WSL).

1. Make the script executable
   ```bash
   chmod +x wyag
   ```
2. Running Commands
   Invoke ```wyag``` using the following syntax:

   ```bash
   ./wyag <command> [options] [arguments]
   ```

   For example:

      - Initialize a new repository
      ```bash
      ./wyag init [directory]
      ```

      Creates a new Git repository in the specified directory (or the current directory if ommitted).

      - Add a File
      ```bash
      ./wyag add <file>
      ```
      Adds a file to the staging area.

      - Commit changes
      ```bash
      ./wyag commit -m "Commit message"
      ```
      Commits staged changes with a message.

      - Show commit log
      ```bash
      ./wyag log
      ```
      Displays the commit history.

      - Show repository status
      ```bash
      ./wyag status
      ```
      Shows the status of the working directory and the staging area.

      - Inspect an Object
      ```bash
      ./wyag cat-file blob <object_hash>
      ```
      Prints the content of a blob object.

      - Hash and store a file
      ```bash
      ./wyag hash-object -w <file>
      ```
      Hashes and stores a file as a blob object.
   
3. Getting help
   To see the available commands and options :

   ```bash
   ./wyag --help
   ```
   Or to help with a specific command:
   ```bash
   ./wyag <command> --help
   ```



## Contributing

   Contributions welcome! Fork the project, make your changes, and open a pull request.
