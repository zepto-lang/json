# json

A minimal JSON library in zepto. It is a stub right now.

It only supports JSON to zepto encoding and is largely undocumented.

## Usage

Usage is pretty simple. There is a file called `test.zp` that shows
the most basic usage example I can think of.

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

Yay, right?

<br/>

*Have fun!*
