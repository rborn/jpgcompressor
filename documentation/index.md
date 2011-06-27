# jpgcompressor Module

## Description

Using UIImageJPEGRepresentation to pass the option to compress image passed as TiBlob

## Accessing the jpgcompressor Module

To access this module from JavaScript, you would do the following:

	var jpgcompressor = require("com.sideshowcoder.jpgcompressor");

## Reference

### jpgcompressor.setCompressFactor

Set the compress factor passed to UIImageJPEGRepresentation

### jpgcompressor.compressFactor

Read the compress factor passed to UIImageJPEGRepresentation

### jpgcompressor.compress

Pass image as Blob to be compressed


## Usage

  jpgcompressor.setCompressFactor(0.5);
  var f = Ti.Filesystem.getFile('test.jpg');
  var img = f.read.blob;
  var compressedImg = jpgcompressor.compress(img);

## Author

Philipp Fehre <philipp.fehre@googlemail.com>
[Sideshowcoder](http://sideshowcoder.com)

## License

Copyright (c) 2011, Philipp Fehre
All rights reserved.

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.