# bobo

KISS static site generator in ~120 lines of POSIX shell and awk.

## Getting Started

```
$ git clone https://github.com/cristianrz/bobo.git
```

### Prerequisites

* `git`
* `smu` as a markdown to html converter, but any converter can be used, just
need to change the `CMD` variable in `./bobo-build-page`.
* `busybox`

### How to use

```
$ ./bobo-init
```

Now edit your website and

```
$ ./bobo-run
```

and you have a local server at `localhost:8080`

## Authors

  - **Cristian Ariza** - [cristianrz](https://github.com/cristianrz)

See also the list of
[contributors](https://github.com/cristianrz/bobo/contributors)
who participated in this project.

## License

See the [LICENSE](LICENSE) file for details

