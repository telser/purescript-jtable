# purescript-jtable

[![Latest release](http://img.shields.io/bower/v/purescript-jtable.svg)](https://github.com/slamdata/purescript-jtable/releases)
[![Build Status](https://travis-ci.org/slamdata/purescript-jtable.svg?branch=master)](https://travis-ci.org/slamdata/purescript-jtable)
[![Dependency Status](https://www.versioneye.com/user/projects/565c3fb34052e80035000053/badge.svg?style=flat)](https://www.versioneye.com/user/projects/565c3fb34052e80035000053)

A small but powerful Purescript library to render arbitrary JSON into HTML tables.

Turn this:

```json
{
  "userId": 8927524,
  "profile": {
    "name":   "Mary Jane",
    "age":    29,
    "gender": "female"
  },
  "comments": [{
    "id":       "F2372BAC",
    "text":     "I concur.",
    "replyTo":  [9817361, "F8ACD164F"],
    "time":     "2015-02-03"
  }, {
    "id":       "GH732AFC",
    "replyTo":  [9654726, "A44124F"],
    "time":     "2015-03-01"
  }]
}
```

Into this:

```
|----------|----------------------------|------------------------------------------------------------|
|          |           profile          |                           comments                         |
|----------|-----------|-----|----------|----------|--------------|---------------------|------------|
|  userId  |    name   | age |  gender  |    id    |     text     |       replyTo       |    time    |
|----------|-----------|-----|----------|----------|--------------|---------------------|------------|
|  8927524 | Mary Jane |  29 |  female  | F2372BAC | I concur.    | 9817361 | F8ACD164F | 2015-02-03 |
|          |           |     |          |----------|--------------|---------------------|------------|
|          |           |     |          | GH732AFC |              | 9654726 | A44124F   | 2015-03-01 |
|----------|-----------|-----|----------|------------------------------------------------------------|
```


## Installation

```
bower install purescript-jtable
```


## Example

See [examples/src/Main.purs](examples/src/Main.purs) for example usage.


## Documentation

Module documentation is published on Pursuit: [http://pursuit.purescript.org/packages/purescript-jtable](http://pursuit.purescript.org/packages/purescript-jtable)
