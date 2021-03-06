## shorten

> A personal URL shortener via GitHub Pages.

Shorten lets you create, view, and manage shortened URLs. All pages are hosted with GitHub Pages and redirection is done with HTML5's [`http-equiv` refresh attribute](https://developer.mozilla.org/en/docs/Web/HTML/Element/meta#attr-http-equiv).

### Demo

![](./.github/shorten.gif)

### Installation

  - Requires Go to be [installed](https://golang.org/doc/install) and [configured](https://golang.org/doc/install#testing).

  - Install with Go:

    ```sh
    $ go get -v github.com/kshvmdn/shorten
    $ shorten --help
    ```

  - Or install directly via source:

    ```sh
    $ git clone https://github.com/kshvmdn/shorten.git $GOPATH/src/github.com/kshvmdn/shorten
    $ cd $_
    $ make install && make
    $ ./shorten --help
    ```

### Usage

  - View the help dialogue by passing the `--help` / `-h` flag. View the specific help dialogue for each command by running `shorten [command] --help`.

    ```
    $ shorten --help
    Create and manage shortened URLs with GitHub Pages.

    Usage:
      shorten [command]

    Available Commands:
      create      Create a new shortened URL.
      export      Print the current config. file.
      help        Help about any command
      import      Import a pre-existing config. file.
      list        Print a list of currently active URLs.
      remove      Remove a shortened URL and delete the associated repository.

    Use "shorten [command] --help" for more information about a command.
    ```

  - On first run, you'll be prompted for a GitHub access token. You can request that [here](https://github.com/settings/tokens). Shorten only requires the `repo`, `user`, and `delete_repo` permissions. Note that your access token will only be stored locally (in `~/.shorten.toml`).

### Contribute

This project is completely open source. Feel free to [open an issue](https://github.com/kshvmdn/shorten/issues) with questions / suggestions / requests or [create a pull request](https://github.com/kshvmdn/shorten/pulls) to contribute!

### License

[MIT](./LICENSE) © Kashav Madan.
