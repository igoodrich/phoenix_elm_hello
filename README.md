# PhoenixElmHello
Simple project that shows phoenix and Elm playing quite nicely together.
Not a lot of work!

### Screenshot
![alt text](https://github.com/igoodrich/phoenix_elm_hello/blob/master/web/static/assets/images/hello_from_elmland.png "Screenshot")

### Motivation
I thought a github project and a diff would be a simplest way to see what should be done.
If you want more of a walk through, check out the helpful blog posts.

### Blog Posts
Based on these helpful blog posts:
* [Alan Gardner's](http://www.cultivatehq.com/posts/phoenix-elm-2/)
* [Brandon Richey's](https://medium.com/@diamondgfx/setting-up-elm-with-phoenix-be3a9f55bac2#.aiom56gn7)

### Versions
* phoenix 1.1.4
* Elm 0.17

### Diff
Short diff of all changes:
[Diff](https://github.com/igoodrich/phoenix_elm_hello/commit/c8442a72fda6f9fe9e4d16a2fb3a992606823241 "Full Diff")

### Instructions

#### Make the Phoenix app
```
1. mix phoenix.new phoenix_elm_hello
1. cd phoenix_elm_hello/
1. mix ecto.create
```

#### Edit / Create a couple files
[Diff](https://github.com/igoodrich/phoenix_elm_hello/commit/c8442a72fda6f9fe9e4d16a2fb3a992606823241 "Full Diff")
4. .gitignore
2. brunch-config.json
1. package.json
1. edit package.json
3. Hello.elm (or whatever)
4. elm-package.json
5. app.js
6. index.html.eex

#### Run the things
```
npm install
mkdir web/elm && touch web/elm/Hello.elm
cd web/elm
elm package install elm-lang/html
cd ../..
mix phoenix.server
```

## Notes
* Changes to your elm file will autocompile (cool!)
* If you add more elm modules, you need to add them to your brunch-config.json (I think)
