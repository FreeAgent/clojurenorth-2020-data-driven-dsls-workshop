# Liner

Liner is a Clojure(script) library for processing command-line arguments.

![Ocean liner](./ocean_liner_photo_by_x1klima.jpg)

## Quick Start

For a `-p 8080` / `--port 8080` flag, you might use:

```clojure
  [ { :flag "p"
      :full "port"
      :help  "the port number your server runs on"
      :coerce "int"
      :default 8000
    }
  ]
```

Liner returns a map, such as:

```clojure
{ :p 8080 }
```

Or, if the argument isn't passed (& there's no default):

```clojure
{ :p nil }
```

## Limitations / Future Work

## Credits

Photo by [https://www.flickr.com/people/x1klima/](https://www.flickr.com/people/x1klima/)