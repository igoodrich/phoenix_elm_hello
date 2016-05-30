# PhoenixElmHello

## Screenshot

## Blog Posts

Check these out for more details.
http://www.cultivatehq.com/posts/phoenix-elm-2/
https://medium.com/@diamondgfx/setting-up-elm-with-phoenix-be3a9f55bac2#.aiom56gn7

## Versions

* phoenix 1.1.4
* Elm 0.17

## Why

Check out how few changes need to be made to get phoenix and elm working together.
I thought a github project and a diff would be useful.

## Diff

Here's the diff.

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
