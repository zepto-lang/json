# json

A minimal JSON library in zepto. It is in alpha right now.

## Usage

Usage is pretty simple. There is a file called `test.zp` that shows
the most basic usage examples I can think of.

Decoding from JSON could look like this:
```clojure
(define x (json:parse
            "{ \"unnamed\": 10,
               'lol': {
                 10: 'hello',
                 11: [1, 2]
               }
             }"))
; this will return a hash-map like so:
; #{lol: #{10: hello, 11: (1 2)}, unnamed: 10, }
```

Encoding to JSON looks like this:
```clojure
(define x (json:dump #{1 (1 2) 3 "something"}))
; this will return a string like so:
; {10: [1, 2], 3: "something"}
```

Yay, right?

<br/>

*Have fun!*
