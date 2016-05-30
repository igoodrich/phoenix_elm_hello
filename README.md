# PhoenixElmHello
Simple project that shows phoenix and Elm playing quite nicely together.
Not a lot of work!
* phoenix 1.1.4
* Elm 0.17

![Screenhot]
(https://github.com/igoodrich/phoenix_elm_hello/blob/master/web/static/assets/images/hello_from_elmland.png)


## Motivation
I thought a github project and a diff would be a simplest way to see what should be done.
If you want more of a walk through, check out the helpful blog posts.

## Links to Helpful Blog Posts
This repo is a condensed version of what's here:
* [Alan Gardner's](http://www.cultivatehq.com/posts/phoenix-elm-2/)
* [Brandon Richey's](https://medium.com/@diamondgfx/setting-up-elm-with-phoenix-be3a9f55bac2#.aiom56gn7)

## Instructions

### Make your phoenix app
```
mix phoenix.new phoenix_elm_hello
cd phoenix_elm_hello/
mix ecto.create
mkdir web/elm
```

### Edit Files
[All the Changes](https://github.com/igoodrich/phoenix_elm_hello/commit/c8442a72fda6f9fe9e4d16a2fb3a992606823241 "Full Diff")

### npm install
```
npm install
```

### elm packgage install
```
cd web/elm
elm package install elm-lang/html
cd ../..
```

### start phoenix
```
mix phoenix.server
```

### [http://localhost:4000] (http://localhost:4000)

![Screenhot]
(https://github.com/igoodrich/phoenix_elm_hello/blob/master/web/static/assets/images/hello_from_elmland.png)

## Notes
* Changes to your elm file will autocompile (cool!)
* If you add more elm modules, you need to add them to your brunch-config.json (I think)
