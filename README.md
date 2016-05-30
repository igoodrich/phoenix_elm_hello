# PhoenixElmHello

## Screenshot
![alt text](https://github.com/igoodrich/phoenix_elm_hello/blob/master/web/static/assets/images/hello_from_elmland.png "Screenshot")

## Blog Posts

### Check these out for more details.
* http://www.cultivatehq.com/posts/phoenix-elm-2/
* https://medium.com/@diamondgfx/setting-up-elm-with-phoenix-be3a9f55bac2#.aiom56gn7

## Versions

* phoenix 1.1.4
* Elm 0.17

## Why

I thought a github project and a diff would be a simplest way to see what should be done.
If you want more of a walk through, check out the helpful blog posts.

## Diff

Here's the diff.
![alt text](https://github.com/igoodrich/phoenix_elm_hello/commit/c8442a72fda6f9fe9e4d16a2fb3a992606823241 "Full Diff")

## Instructions

```
mix phoenix.new phoenix_elm_hello
cd phoenix_elm_hello/
mix ecto.create
```

[edit package.json, brunch-config.json -- see diff]

```
npm install
mkdir web/elm && touch web/elm/Hello.elm
```

[edit Hello.elm -- see diff]

```
cd web/elm
elm package install elm-lang/html
cd ../..
mix phoenix.server
```

## Notes
Changes to your elm file will autocompile (cool!)
If you add more elm modules, you need to add them to your brunch-config.json (I think)
