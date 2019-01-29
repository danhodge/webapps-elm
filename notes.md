2. Hello, Elm!

Starting a new Elm project

Run from root directory of project
% elm-package install

(adds an elm-package.json file & the elm-stuff directory)

Elm Reactor
% elm-reactor

(then navigate to localhost:8000)

Compiling Elm to JS
% elm-make <File.elm> --output=<file.js>

Elm Watch
elm-live <File.elm> --open --output=<file.js>

Elm Repl
% elm-repl

Functions
parenthesies are optional, only should be used for grouping
> String.repeat 3 (String.toUpper "hi")

Pipeline is better and more idiomatic
- when used, the previous expression is passed in as the last argument
  to the next

"hi"
    |> String.toUpper
    |> String.repeat 3

type declarations
T -> F (function takes a T returns an F)
T -> F -> G (function takes a T returns a function that takes an F and
returns a G)

Defining Functions
<function_name> <arg1> ... <argN> =
    <function_body>

Anonymous Functions
fn = \<arg1> ... <argN> -> <function_body>

Types
Uppercase name (i.e. List) = a type name
Lowercase name (i.e. List a) = a type variable
