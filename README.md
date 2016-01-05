# GoDiesel

GoDiesel is an embeddable scheme REPL focused on Domain Specific Language
creation. It is written in Go and a great Go interface. It was derived from
and inspired by [Howard Mao's terrific Glisp project](https://github.com/zhemao/glisp).

GoDiesel's features have evolved to the point where it is a now distinct dialect.
This was done to support certain critical features like raw string literals,
to support for certain scheme and clojure idioms, and to make it easier
to use as a library within a larger program.

It is ideally suited for driving complex configurations and providng
your project with a domain specific language customized to your challenges.

Brief list of implemented features.

 * [x] Small code base, easy to extend and integrate.
 * [x] Float, Int, Char, String, Symbol, List, Array, and Hash datatypes
 * [x] Arithmetic (`+`, `-`, `*`, `/`, `mod`, `**`)
 * [x] Shift Operators (`sll`, `srl`, `sra`)
 * [x] Bitwise operations (`bit-and`, `bit-or`, `bit-xor`)
 * [x] Comparison operations (`<`, `>`, `<=`, `>=`, `==`, `!=`, and `not=`)
 * [x] Short-circuit boolean operators (`and` and `or`)
 * [x] Conditionals (`cond`)
 * [x] Lambdas (`fn`)
 * [x] Bindings (`def`, `defn`, and `let`)
 * [x] Standalone and embedable REPL.
 * [x] Tail-call optimization
 * [x] Go API
 * [x] Macro System
 * [x] Syntax quoting -- with caret `^()` instead of backtick.
 * [x] Channel and goroutine support
 * [x] Pre- and Post- function call hooks

Features in GoDiesel v0.9.3:

 * [x] Clojure like threading `(-> hash field1: field2:)` and `(:field hash)` selection
 * [x] Raw bytes type `(raw string)` lets you do zero-copy []byte manipulation
 * [x] Record definitions `(defmap)`
 * [x] Read external files with `(req path-to-file)`
 * [x] Go style raw string literals
 * [x] JSON and Msgpack interop: serialization and deserialization
 
The full documentation can be found in the [Wiki](https://github.com/glycerine/glisp/wiki).
