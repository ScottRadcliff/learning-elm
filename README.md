# Learning the Elm Programming Language
[Elm-lang](http://elm-lang.org/)

This is a learning experience in Elm Language. I am an open complainer of modern JavaScript and what it brings to web development. I like the idea of writing in a functional language to control the front-end code.


Not sure how I feel about the HTML/CSS parts yet.


## Helpful Links
* [Elm Packages](http://package.elm-lang.org/)

## Getting Started
When compiling my first program [HelloWorld](https://github.com/ScottRadcliff/learning-elm/tree/master/HelloWorld), all of the instructions for grabbing the HTML package didn't work. Most things I found told me to install `evancz/elm-html`. That must not exist anymore (as of 5/14/16). It looks like that package is part of `elm-lang` now.

`elm-package install elm-lang/html`


## Notes
When looking to add something from a package, [http://package.elm-lang.org/](http://package.elm-lang.org/) has really good documentation, but it's a little different than I'm used to. The type annotation lists things that are required and must be included. I don't think any parameters are optional.

For h1, I needed `h1 [] [ text "Heading" ]`. Leaving out `[]` resulted in an error on the next line. I also needed to remember to add h1 to the import statement. The program will complain about an unknown variable.

### Updating Records
When a record has a pipe in it, it is updating the record before the pipe with the what is after the pipe.

`{ model | content = newContent }`
