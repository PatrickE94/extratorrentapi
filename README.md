# ExtraTorrent API

Simple wrapper around extratorrent's RSS feed.

Using [got library](https://github.com/sindresorhus/got)

## Methods
```
var extratorrent = require('extratorrent');

extratorrent
  .search('query') // Promise style
  .then(function(torrents) {
    /**
     * [
     *  {
     *    title: '',
     *    link: '',
     *    hash: '',
     *    torrent: '',
     *    seeds: NaN,
     *    leechs: NaN,
     *    peers: NaN,
     *    size: NaN,
     *    magnetLink: ''
     *  }
     * ]
     */
  })
  .catch(function(error) {
    console.error(error);
  });

  // Other API's
  extratorrent.popular();
  extratorrent.today();
  extratorrent.yesterday();
  extratorrent.category();
```

## LICENSE

The MIT License (MIT)

Copyright (c) 2015 Patrick Engström

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
