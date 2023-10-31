# Zonx Docs Example Site

This repository offers a multilingual example site using the [Zonx Docs](https://github.com/zonxorg/zonxdocs) Hugo theme.

# Using

1. [Install Hugo](https://gohugo.io/overview/installing/)
2. Clone this repository

    ```bash
    $ git clone --depth 1 https://github.com/zonxorg/zonxdocs zonxdocs
    $ cd zonxdocs/exampleSite
    ```
3. Run Hugo server.

    ```bash
    $ hugo server
    ```
## Notes:

The `exampleSite` functions by using the Hugo [`replace`](https://gohugo.io/hugo-modules/use-modules/#make-and-test-changes-in-a-module) directive (in [`go.mod`](go.mod#L10)) to point the default `zonxdocs` module path, `github.com/zonxorg/zonxdocs`, to the local directory above where the theme is cloned:

```go
// go.mod
...

replace github.com/zonxorg/zonxdocs => ../
```
