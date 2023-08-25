# mkpwd

> A simple password generator written in Python, to create strong random passwords.

- - -

[![][mainBadge]][main] [![GitLab release][latestBadge]][latest]

![][pythonVersion] ![][licenseBadge]


## Install

Install the file to `/usr/local/bin`, or to any other location. Just make sure it's added to `PATH`.

```bash
$ cd /path/to/mkpwd
$ sudo install -v -m755 -o0 -g0 mkpwd /usr/local/bin
```

## Usage

Use `mkpwd -h` to bring the help.

```txt
Usage:
    mkpwd [ -hq ] [ size ] [ nr of pwds ]
    mkpwd           Enter a number at the prompt
    mkpwd 24        24 character pwd
    mkpwd 36 10     10x 36 character pwd

Options:
    -h              Display this help.
    -q              Quiet mode (only the pwd(s) in output).
                    Useful for scripting.
```

There's a _“Settings & text strings”_ section early in the script where you can change the defaults, &/or translate the text strings if you'd prefer that.


## Sample output

Here are a few examples of how it looks.

```bash
$ mkpwd
:: Password length [default: 18]: 24
mkpwd:  bU7Hc<Bv-}lpF1!Q8:dW6f3M
$ mkpwd 24
mkpwd:  |i20/(5QBaqH-@7i4TrXFtbU
$ mkpwd 24 3
mkpwd #1:   s)P5Qz6jp4\SgH<'r#A1pB4M
mkpwd #2:   p]ZB5x8I9GuA>3nEa4vJ=.u>
mkpwd #3:   eVYrN4=Zj2W0!VwsrI8/9{?e
```


#### Quiet mode

Use `mkpwd -q` to suppress anything but the passwords. This is great when scripting - like using it with, example: `mkpwd -q 18` will get you 1 password, 18 characters long.

```bash
# one password
$ mkpwd -q 18
=)b3aR_0V6s1BavZ*C

# 3 passwords
$ mkpwd -q 18 3
T:6O08bEqy)I3|\lXs
Z9VKps;6lB1x2_%cD=
xK,q50LJ;7]s3OCw~g
```


## License, credits and copyright

![][licenseBadge]


## Contributing

1. Fork it (<https://gitlab.com/iefdev/mkpwd/forks/new>)
2. Create your feature branch (`git switch -c feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Merge Request


## Author notes

-   **[2023-08-25]** Making a tag/release (v0.6.0) of this. Not that it's really needed,
    but as good practice. In case someone needs/wants to use the script - it's easier to use
    releases, and keep it updated that way.

**Pylint**

-   **[2023-08-18]** 10.00/10 (pylint 2.4.4, Python 3.6.8).

- - -

 

If you have any feedback, suggestions? Please, use the Issues, Merge Requests, send an email or post me at X.

· Eric ([@iefdev][x])

<!-- Markdown: link & image dfn's -->
[pythonVersion]: https://img.shields.io/badge/python-3.6+-FFD343.svg?logo=python&logoColor=FFD343&labelColor=3D75AD&style=plastic "Python 3.6+"
[licenseBadge]: https://img.shields.io/badge/license-GPL--3.0--or--later-C00?style=plastic "GPL v3.0 or later"
[mainBadge]: https://img.shields.io/badge/main-v0.99-778899.svg?logo=gitlab&style=plastic
[latestBadge]: https://img.shields.io/badge/latest-v0.6.0-blue.svg?logo=gitlab&style=plastic
[latest]: https://gitlab.com/iefdev/mkpwd/-/releases/ "Latest tag/release"
[main]: https://gitlab.com/iefdev/mkpwd/ "main branch"
[x]: https://twitter.com/iefdev

