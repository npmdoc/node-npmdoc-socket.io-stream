# api documentation for  [socket.io-stream (v0.9.1)](https://github.com/nkzawa/socket.io-stream#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-socket.io-stream.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-socket.io-stream) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-socket.io-stream.svg)](https://travis-ci.org/npmdoc/node-npmdoc-socket.io-stream)
#### stream for socket.io

[![NPM](https://nodei.co/npm/socket.io-stream.png?downloads=true)](https://www.npmjs.com/package/socket.io-stream)

[![apidoc](https://npmdoc.github.io/node-npmdoc-socket.io-stream/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-socket.io-stream_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-socket.io-stream/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-socket.io-stream/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-socket.io-stream/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Naoyuki Kanezawa",
        "email": "naoyuki.kanezawa@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/nkzawa/socket.io-stream/issues"
    },
    "contributors": [
        {
            "name": "Naoyuki Kanezawa",
            "email": "naoyuki.kanezawa@gmail.com"
        },
        {
            "name": "Aaron O'Mullan",
            "email": "aaron.omullan@friendco.de"
        }
    ],
    "dependencies": {
        "component-bind": "~1.0.0",
        "debug": "~2.2.0"
    },
    "description": "stream for socket.io",
    "devDependencies": {
        "blob": "0.0.4",
        "browserify": "~13.1.0",
        "expect.js": "~0.3.1",
        "mocha": "~3.0.2",
        "socket.io": "~1.4.8",
        "socket.io-client": "~1.4.8",
        "zuul": "~3.11.1",
        "zuul-ngrok": "~4.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "421258316288b83ac693b0d43efd09d6d43aba97",
        "tarball": "https://registry.npmjs.org/socket.io-stream/-/socket.io-stream-0.9.1.tgz"
    },
    "gitHead": "8feef9e9ce296ec87e471731735abc6982e4158d",
    "homepage": "https://github.com/nkzawa/socket.io-stream#readme",
    "keywords": [
        "stream",
        "socket.io",
        "binary",
        "file",
        "upload",
        "download"
    ],
    "maintainers": [
        {
            "name": "nkzawa",
            "email": "naoyuki.kanezawa@gmail.com"
        }
    ],
    "name": "socket.io-stream",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/nkzawa/socket.io-stream.git"
    },
    "scripts": {
        "prepublish": "make build",
        "test": "make test"
    },
    "version": "0.9.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module socket.io-stream](#apidoc.module.socket.io-stream)
1.  boolean <span class="apidocSignatureSpan">socket.io-stream.</span>forceBase64
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.IOStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.Socket)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>createBlobReadStream (blob, options)](#apidoc.element.socket.io-stream.createBlobReadStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>createStream (options)](#apidoc.element.socket.io-stream.createStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.io-stream.Buffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.IOStream (options)](#apidoc.element.socket.io-stream.io-stream.IOStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Socket (sio, options)](#apidoc.element.socket.io-stream.io-stream.Socket)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.blob_read_stream (blob, options)](#apidoc.element.socket.io-stream.io-stream.blob_read_stream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.socket_io_stream (sio, options)](#apidoc.element.socket.io-stream.io-stream.socket_io_stream)
1.  object <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Buffer.prototype
1.  object <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.IOStream.prototype
1.  object <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Socket.prototype
1.  object <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.blob_read_stream.prototype
1.  object <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.parser

#### [module socket.io-stream.Buffer](#apidoc.module.socket.io-stream.Buffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer.Buffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>alloc (size, fill, encoding)](#apidoc.element.socket.io-stream.Buffer.alloc)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>allocUnsafe (size)](#apidoc.element.socket.io-stream.Buffer.allocUnsafe)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>allocUnsafeSlow (size)](#apidoc.element.socket.io-stream.Buffer.allocUnsafeSlow)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>byteLength (string, encoding)](#apidoc.element.socket.io-stream.Buffer.byteLength)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>compare (a, b)](#apidoc.element.socket.io-stream.Buffer.compare)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>concat (list, length)](#apidoc.element.socket.io-stream.Buffer.concat)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>from (value, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer.from)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>isBuffer (b)](#apidoc.element.socket.io-stream.Buffer.isBuffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>isEncoding (encoding)](#apidoc.element.socket.io-stream.Buffer.isEncoding)
1.  number <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>poolSize

#### [module socket.io-stream.Buffer.prototype](#apidoc.module.socket.io-stream.Buffer.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.socket.io-stream.Buffer.prototype.asciiSlice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.socket.io-stream.Buffer.prototype.asciiWrite)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>base64Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.base64Slice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>base64Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.base64Write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.socket.io-stream.Buffer.prototype.compare)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>copy ()](#apidoc.element.socket.io-stream.Buffer.prototype.copy)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>equals (b)](#apidoc.element.socket.io-stream.Buffer.prototype.equals)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.fill)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>hexSlice ()](#apidoc.element.socket.io-stream.Buffer.prototype.hexSlice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>hexWrite ()](#apidoc.element.socket.io-stream.Buffer.prototype.hexWrite)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.includes)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.indexOf)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>inspect ()](#apidoc.element.socket.io-stream.Buffer.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.lastIndexOf)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.latin1Slice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>latin1Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.latin1Write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readDoubleBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readDoubleLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readFloatBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readFloatLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt16BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt16LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt32BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt32LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt8)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readIntBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readIntLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt16BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt16LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt32BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt32LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt8)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUIntBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUIntLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>slice (start, end)](#apidoc.element.socket.io-stream.Buffer.prototype.slice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap16 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap16)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap32 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap32)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap64 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap64)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>toJSON ()](#apidoc.element.socket.io-stream.Buffer.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>toString ()](#apidoc.element.socket.io-stream.Buffer.prototype.toString)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.ucs2Slice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.ucs2Write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.utf8Slice)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>utf8Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.utf8Write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeFloatBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeFloatLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt16BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt16LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt32BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt32LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt8)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeIntBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeIntLE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32BE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32LE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt8)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUIntBE)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUIntLE)

#### [module socket.io-stream.IOStream](#apidoc.module.socket.io-stream.IOStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.IOStream.IOStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.</span>super_ (options)](#apidoc.element.socket.io-stream.IOStream.super_)

#### [module socket.io-stream.IOStream.prototype](#apidoc.module.socket.io-stream.IOStream.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_done ()](#apidoc.element.socket.io-stream.IOStream.prototype._done)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_end ()](#apidoc.element.socket.io-stream.IOStream.prototype._end)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onend ()](#apidoc.element.socket.io-stream.IOStream.prototype._onend)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onerror (err)](#apidoc.element.socket.io-stream.IOStream.prototype._onerror)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onfinish ()](#apidoc.element.socket.io-stream.IOStream.prototype._onfinish)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onread (size)](#apidoc.element.socket.io-stream.IOStream.prototype._onread)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onwrite (chunk, encoding, callback)](#apidoc.element.socket.io-stream.IOStream.prototype._onwrite)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_read (size)](#apidoc.element.socket.io-stream.IOStream.prototype._read)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.socket.io-stream.IOStream.prototype._write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>destroy ()](#apidoc.element.socket.io-stream.IOStream.prototype.destroy)

#### [module socket.io-stream.Socket](#apidoc.module.socket.io-stream.Socket)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.Socket.Socket)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.</span>super_ ()](#apidoc.element.socket.io-stream.Socket.super_)
1.  object <span class="apidocSignatureSpan">socket.io-stream.Socket.</span>events
1.  string <span class="apidocSignatureSpan">socket.io-stream.Socket.</span>event

#### [module socket.io-stream.Socket.prototype](#apidoc.module.socket.io-stream.Socket.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_end (id)](#apidoc.element.socket.io-stream.Socket.prototype._end)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_error (id, err)](#apidoc.element.socket.io-stream.Socket.prototype._error)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_ondecode (stream)](#apidoc.element.socket.io-stream.Socket.prototype._ondecode)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_ondisconnect ()](#apidoc.element.socket.io-stream.Socket.prototype._ondisconnect)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onencode (stream)](#apidoc.element.socket.io-stream.Socket.prototype._onencode)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onend (id)](#apidoc.element.socket.io-stream.Socket.prototype._onend)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onerror (id, message)](#apidoc.element.socket.io-stream.Socket.prototype._onerror)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onread (id, size)](#apidoc.element.socket.io-stream.Socket.prototype._onread)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onstream (type, listener)](#apidoc.element.socket.io-stream.Socket.prototype._onstream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onwrite (id, chunk, encoding, callback)](#apidoc.element.socket.io-stream.Socket.prototype._onwrite)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_read (id, size)](#apidoc.element.socket.io-stream.Socket.prototype._read)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_stream (type)](#apidoc.element.socket.io-stream.Socket.prototype._stream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_write (id, chunk, encoding, callback)](#apidoc.element.socket.io-stream.Socket.prototype._write)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>cleanup (id)](#apidoc.element.socket.io-stream.Socket.prototype.cleanup)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>emit (type)](#apidoc.element.socket.io-stream.Socket.prototype.emit)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>on (type, listener)](#apidoc.element.socket.io-stream.Socket.prototype.on)

#### [module socket.io-stream.blob_read_stream](#apidoc.module.socket.io-stream.blob_read_stream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>blob_read_stream (blob, options)](#apidoc.element.socket.io-stream.blob_read_stream.blob_read_stream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.</span>super_ (options)](#apidoc.element.socket.io-stream.blob_read_stream.super_)

#### [module socket.io-stream.blob_read_stream.prototype](#apidoc.module.socket.io-stream.blob_read_stream.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_onerror (e)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._onerror)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_onload (e)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._onload)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_read (size)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._read)

#### [module socket.io-stream.parser](#apidoc.module.socket.io-stream.parser)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.parser.</span>Decoder ()](#apidoc.element.socket.io-stream.parser.Decoder)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.parser.</span>Encoder ()](#apidoc.element.socket.io-stream.parser.Encoder)

#### [module socket.io-stream.socket_io_stream](#apidoc.module.socket.io-stream.socket_io_stream)
1.  boolean <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>forceBase64
1.  [function <span class="apidocSignatureSpan">socket.io-stream.</span>socket_io_stream (sio, options)](#apidoc.element.socket.io-stream.socket_io_stream.socket_io_stream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.socket_io_stream.Buffer)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.socket_io_stream.IOStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.socket_io_stream.Socket)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>createBlobReadStream (blob, options)](#apidoc.element.socket.io-stream.socket_io_stream.createBlobReadStream)
1.  [function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>createStream (options)](#apidoc.element.socket.io-stream.socket_io_stream.createStream)



# <a name="apidoc.module.socket.io-stream"></a>[module socket.io-stream](#apidoc.module.socket.io-stream)

#### <a name="apidoc.element.socket.io-stream.Buffer"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
...

### ss.Buffer

[Node Buffer](https://nodejs.org/api/buffer.html) class to use on browser, which is exposed for convenience. On Node environment
, you should just use normal 'Buffer'.

'''js
var stream = ss.createStream();
stream.write(new ss.Buffer([0, 1, 2]));
'''

## License

MIT
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.IOStream)
- description and source-code
```javascript
function IOStream(options) {
  if (!(this instanceof IOStream)) {
    return new IOStream(options);
  }

  IOStream.super_.call(this, options);

  this.options = options;
  this.id = uuid();
  this.socket = null;

  // Buffers
  this.pushBuffer = [];
  this.writeBuffer = [];

  // Op states
  this._readable = false;
  this._writable = false;
  this.destroyed = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  this.on('finish', this._onfinish);
  this.on('end', this._onend);
  this.on('error', this._onerror);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.Socket)
- description and source-code
```javascript
function Socket(sio, options) {
  if (!(this instanceof Socket)) {
    return new Socket(sio, options);
  }

  EventEmitter.call(this);

  options = options || {};

  this.sio = sio;
  this.forceBase64 = !!options.forceBase64;
  this.streams = {};
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();

  var eventName = exports.event;
  sio.on(eventName, bind(this, emit));
  sio.on(eventName + '-read', bind(this, '_onread'));
  sio.on(eventName + '-write', bind(this, '_onwrite'));
  sio.on(eventName + '-end', bind(this, '_onend'));
  sio.on(eventName + '-error', bind(this, '_onerror'));
  sio.on('error', bind(this, emit, 'error'));
  sio.on('disconnect', bind(this, '_ondisconnect'));

  this.encoder.on('stream', bind(this, '_onencode'));
  this.decoder.on('stream', bind(this, '_ondecode'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.createBlobReadStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>createBlobReadStream (blob, options)](#apidoc.element.socket.io-stream.createBlobReadStream)
- description and source-code
```javascript
createBlobReadStream = function (blob, options) {
  return new BlobReadStream(blob, options);
}
```
- example usage
```shell
...

  $('#file').change(function(e) {
    var file = e.target.files[0];
    var stream = ss.createStream();

    // upload a file to the server.
    ss(socket).emit('file', stream, {size: file.size});
    ss.createBlobReadStream(file).pipe(stream);
  });
});
</script>
'''

#### Upload progress
...
```

#### <a name="apidoc.element.socket.io-stream.createStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>createStream (options)](#apidoc.element.socket.io-stream.createStream)
- description and source-code
```javascript
createStream = function (options) {
  return new IOStream(options);
}
```
- example usage
```shell
...
Client:

'''js
var io = require('socket.io-client');
var ss = require('socket.io-stream');

var socket = io.connect('http://example.com/user');
var stream = ss.createStream();
var filename = 'profile.jpg';

ss(socket).emit('profile-image', stream, {name: filename});
fs.createReadStream(filename).pipe(stream);
'''

You can stream data from a client to server, and vice versa.
...
```

#### <a name="apidoc.element.socket.io-stream.io-stream.Buffer"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.io-stream.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.io-stream.IOStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.IOStream (options)](#apidoc.element.socket.io-stream.io-stream.IOStream)
- description and source-code
```javascript
function IOStream(options) {
  if (!(this instanceof IOStream)) {
    return new IOStream(options);
  }

  IOStream.super_.call(this, options);

  this.options = options;
  this.id = uuid();
  this.socket = null;

  // Buffers
  this.pushBuffer = [];
  this.writeBuffer = [];

  // Op states
  this._readable = false;
  this._writable = false;
  this.destroyed = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  this.on('finish', this._onfinish);
  this.on('end', this._onend);
  this.on('error', this._onerror);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.io-stream.Socket"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.Socket (sio, options)](#apidoc.element.socket.io-stream.io-stream.Socket)
- description and source-code
```javascript
function Socket(sio, options) {
  if (!(this instanceof Socket)) {
    return new Socket(sio, options);
  }

  EventEmitter.call(this);

  options = options || {};

  this.sio = sio;
  this.forceBase64 = !!options.forceBase64;
  this.streams = {};
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();

  var eventName = exports.event;
  sio.on(eventName, bind(this, emit));
  sio.on(eventName + '-read', bind(this, '_onread'));
  sio.on(eventName + '-write', bind(this, '_onwrite'));
  sio.on(eventName + '-end', bind(this, '_onend'));
  sio.on(eventName + '-error', bind(this, '_onerror'));
  sio.on('error', bind(this, emit, 'error'));
  sio.on('disconnect', bind(this, '_ondisconnect'));

  this.encoder.on('stream', bind(this, '_onencode'));
  this.decoder.on('stream', bind(this, '_ondecode'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.io-stream.blob_read_stream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.blob_read_stream (blob, options)](#apidoc.element.socket.io-stream.io-stream.blob_read_stream)
- description and source-code
```javascript
function BlobReadStream(blob, options) {
  if (!(this instanceof BlobReadStream)) {
    return new BlobReadStream(blob, options);
  }

  Readable.call(this, options);

  options = options || {};
  this.blob = blob;
  this.slice = blob.slice || blob.webkitSlice || blob.mozSlice;
  this.start = 0;
  this.sync = options.synchronous || false;

  var fileReader;

  if (options.synchronous) {
    fileReader = this.fileReader = new FileReaderSync();
  } else {
    fileReader = this.fileReader = new FileReader();
  }

  fileReader.onload = bind(this, '_onload');
  fileReader.onerror = bind(this, '_onerror');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.io-stream.socket_io_stream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>io-stream.socket_io_stream (sio, options)](#apidoc.element.socket.io-stream.io-stream.socket_io_stream)
- description and source-code
```javascript
function lookup(sio, options) {
  options = options || {};
  if (null == options.forceBase64) {
    options.forceBase64 = exports.forceBase64;
  }

  if (!sio._streamSocket) {
    sio._streamSocket = new Socket(sio, options);
  }
  return sio._streamSocket;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io-stream.Buffer"></a>[module socket.io-stream.Buffer](#apidoc.module.socket.io-stream.Buffer)

#### <a name="apidoc.element.socket.io-stream.Buffer.Buffer"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      );
    }
    return Buffer.allocUnsafe(arg);
  }
  return Buffer.from(arg, encodingOrOffset, length);
}
```
- example usage
```shell
...

### ss.Buffer

[Node Buffer](https://nodejs.org/api/buffer.html) class to use on browser, which is exposed for convenience. On Node environment
, you should just use normal 'Buffer'.

'''js
var stream = ss.createStream();
stream.write(new ss.Buffer([0, 1, 2]));
'''

## License

MIT
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.alloc"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>alloc (size, fill, encoding)](#apidoc.element.socket.io-stream.Buffer.alloc)
- description and source-code
```javascript
alloc = function (size, fill, encoding) {
  assertSize(size);
  if (size > 0 && fill !== undefined) {
    // Since we are filling anyway, don't zero fill initially.
    // Only pay attention to encoding if it's a string. This
    // prevents accidentally sending in a number that would
    // be interpretted as a start offset.
    if (typeof encoding !== 'string')
      encoding = undefined;
    return createUnsafeBuffer(size).fill(fill, encoding);
  }
  return new FastBuffer(size);
}
```
- example usage
```shell
...

var buffer = require('buffer');
var Buffer = buffer.Buffer;
var SlowBuffer = buffer.SlowBuffer;
var MAX_LEN = buffer.kMaxLength || 2147483647;
exports.alloc = function alloc(size, fill, encoding) {
if (typeof Buffer.alloc === 'function') {
  return Buffer.alloc(size, fill, encoding);
}
if (typeof encoding === 'number') {
  throw new TypeError('encoding must not be number');
}
if (typeof size !== 'number') {
  throw new TypeError('size must be a number');
}
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.allocUnsafe"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>allocUnsafe (size)](#apidoc.element.socket.io-stream.Buffer.allocUnsafe)
- description and source-code
```javascript
allocUnsafe = function (size) {
  assertSize(size);
  return allocate(size);
}
```
- example usage
```shell
...
} else {
  buf.fill(_fill);
}
return buf;
}
exports.allocUnsafe = function allocUnsafe(size) {
if (typeof Buffer.allocUnsafe === 'function') {
  return Buffer.allocUnsafe(size);
}
if (typeof size !== 'number') {
  throw new TypeError('size must be a number');
}
if (size > MAX_LEN) {
  throw new RangeError('size is too large');
}
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.allocUnsafeSlow"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>allocUnsafeSlow (size)](#apidoc.element.socket.io-stream.Buffer.allocUnsafeSlow)
- description and source-code
```javascript
allocUnsafeSlow = function (size) {
  assertSize(size);
  return createUnsafeBuffer(size);
}
```
- example usage
```shell
...
  }
}

throw new TypeError('First argument must be a string, Buffer, ' + 'ArrayBuffer, Array, or array-like object.');
}
exports.allocUnsafeSlow = function allocUnsafeSlow(size) {
if (typeof Buffer.allocUnsafeSlow === 'function') {
  return Buffer.allocUnsafeSlow(size);
}
if (typeof size !== 'number') {
  throw new TypeError('size must be a number');
}
if (size >= MAX_LEN) {
  throw new RangeError('size is too large');
}
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.byteLength"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>byteLength (string, encoding)](#apidoc.element.socket.io-stream.Buffer.byteLength)
- description and source-code
```javascript
function byteLength(string, encoding) {
  if (typeof string !== 'string') {
    if (ArrayBuffer.isView(string) || isArrayBuffer(string) ||
        isSharedArrayBuffer(string)) {
      return string.byteLength;
    }

    string = '' + string;
  }

  var len = string.length;
  if (len === 0)
    return 0;

  // Use a for loop to avoid recursion
  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'ascii':
      case 'latin1':
      case 'binary':
        return len;

      case 'utf8':
      case 'utf-8':
      case undefined:
        return binding.byteLengthUtf8(string);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return len * 2;

      case 'hex':
        return len >>> 1;

      case 'base64':
        return base64ByteLength(string, len);

      default:
        // The C++ binding defaulted to UTF8, we should too.
        if (loweredCase)
          return binding.byteLengthUtf8(string);

        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.compare"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>compare (a, b)](#apidoc.element.socket.io-stream.Buffer.compare)
- description and source-code
```javascript
function compare(a, b) {
  if (!(a instanceof Buffer) ||
      !(b instanceof Buffer)) {
    throw new TypeError('Arguments must be Buffers');
  }

  if (a === b) {
    return 0;
  }

  return binding.compare(a, b);
}
```
- example usage
```shell
...
if (arguments.length === 0) return utf8Slice(this, 0, length)
return slowToString.apply(this, arguments)
}

Buffer.prototype.equals = function equals (b) {
if (!Buffer.isBuffer(b)) throw new TypeError('Argument must be a Buffer')
if (this === b) return true
return Buffer.compare(this, b) === 0
}

Buffer.prototype.inspect = function inspect () {
var str = ''
var max = exports.INSPECT_MAX_BYTES
if (this.length > 0) {
  str = this.toString('hex', 0, max).match(/.{2}/g).join(' ')
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.concat"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>concat (list, length)](#apidoc.element.socket.io-stream.Buffer.concat)
- description and source-code
```javascript
concat = function (list, length) {
  var i;
  if (!Array.isArray(list))
    throw new TypeError('"list" argument must be an Array of Buffers');

  if (list.length === 0)
    return new FastBuffer();

  if (length === undefined) {
    length = 0;
    for (i = 0; i < list.length; i++)
      length += list[i].length;
  } else {
    length = length >>> 0;
  }

  var buffer = Buffer.allocUnsafe(length);
  var pos = 0;
  for (i = 0; i < list.length; i++) {
    var buf = list[i];
    if (!Buffer.isBuffer(buf))
      throw new TypeError('"list" argument must be an Array of Buffers');
    buf.copy(buffer, pos);
    pos += buf.length;
  }

  // Note: 'length' is always equal to 'buffer.length' at this point
  if (pos < length) {
    // Zero-fill the remaining bytes if the specified 'length' was more than
    // the actual total length, i.e. if we have some remaining allocated bytes
    // there were not initialized.
    buffer.fill(0, pos, length);
  }

  return buffer;
}
```
- example usage
```shell
...
     args = self.decoder.decode(args);
     ack.apply(this, args);
   };
 }

 args = this.encoder.encode(args);
 var sio = this.sio;
 sio.emit.apply(sio, [exports.event, type].concat(args));
};

/**
* Notifies the read event.
*
* @api private
*/
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.from"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>from (value, encodingOrOffset, length)](#apidoc.element.socket.io-stream.Buffer.from)
- description and source-code
```javascript
from = function (value, encodingOrOffset, length) {
  if (typeof value === 'number')
    throw new TypeError('"value" argument must not be a number');

  if (isArrayBuffer(value) || isSharedArrayBuffer(value))
    return fromArrayBuffer(value, encodingOrOffset, length);

  if (typeof value === 'string')
    return fromString(value, encodingOrOffset);

  return fromObject(value);
}
```
- example usage
```shell
...
if (size > MAX_LEN) {
  throw new RangeError('size is too large');
}
return new Buffer(size);
}
exports.from = function from(value, encodingOrOffset, length) {
if (typeof Buffer.from === 'function' && (!global.Uint8Array || Uint8Array.from !== Buffer.from)) {
  return Buffer.from(value, encodingOrOffset, length);
}
if (typeof value === 'number') {
  throw new TypeError('"value" argument must not be a number');
}
if (typeof value === 'string') {
  return new Buffer(value, encodingOrOffset);
}
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.isBuffer"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>isBuffer (b)](#apidoc.element.socket.io-stream.Buffer.isBuffer)
- description and source-code
```javascript
function isBuffer(b) {
  return b instanceof Buffer;
}
```
- example usage
```shell
...

/**
 * Requests to write a chunk.
 *
 * @api private
 */
Socket.prototype._write = function(id, chunk, encoding, callback) {
if (Buffer.isBuffer(chunk)) {
  if (this.forceBase64) {
    encoding = 'base64';
    chunk = chunk.toString(encoding);
  } else if (!global.Buffer) {
    // socket.io can't handle Buffer when using browserify.
    if (chunk.toArrayBuffer) {
      chunk = chunk.toArrayBuffer();
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.isEncoding"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.</span>isEncoding (encoding)](#apidoc.element.socket.io-stream.Buffer.isEncoding)
- description and source-code
```javascript
isEncoding = function (encoding) {
  return typeof encoding === 'string' &&
         typeof internalUtil.normalizeEncoding(encoding) === 'string';
}
```
- example usage
```shell
...
}

function fromString (that, string, encoding) {
if (typeof encoding !== 'string' || encoding === '') {
  encoding = 'utf8'
}

if (!Buffer.isEncoding(encoding)) {
  throw new TypeError('"encoding" must be a valid string encoding')
}

var length = byteLength(string, encoding) | 0
that = createBuffer(that, length)

var actual = that.write(string, encoding)
...
```



# <a name="apidoc.module.socket.io-stream.Buffer.prototype"></a>[module socket.io-stream.Buffer.prototype](#apidoc.module.socket.io-stream.Buffer.prototype)

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.asciiSlice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>asciiSlice ()](#apidoc.element.socket.io-stream.Buffer.prototype.asciiSlice)
- description and source-code
```javascript
function asciiSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.asciiWrite"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>asciiWrite ()](#apidoc.element.socket.io-stream.Buffer.prototype.asciiWrite)
- description and source-code
```javascript
function asciiWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.base64Slice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>base64Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.base64Slice)
- description and source-code
```javascript
function base64Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.base64Write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>base64Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.base64Write)
- description and source-code
```javascript
function base64Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.compare"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>compare (target, start, end, thisStart, thisEnd)](#apidoc.element.socket.io-stream.Buffer.prototype.compare)
- description and source-code
```javascript
function compare(target, start, end, thisStart, thisEnd) {

  if (!(target instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');
  if (arguments.length === 1)
    return compare_(this, target);

  if (start === undefined)
    start = 0;
  else if (start < 0)
    throw new RangeError('out of range index');
  else
    start >>>= 0;

  if (end === undefined)
    end = target.length;
  else if (end > target.length)
    throw new RangeError('out of range index');
  else
    end >>>= 0;

  if (thisStart === undefined)
    thisStart = 0;
  else if (thisStart < 0)
    throw new RangeError('out of range index');
  else
    thisStart >>>= 0;

  if (thisEnd === undefined)
    thisEnd = this.length;
  else if (thisEnd > this.length)
    throw new RangeError('out of range index');
  else
    thisEnd >>>= 0;

  if (thisStart >= thisEnd)
    return (start >= end ? 0 : -1);
  else if (start >= end)
    return 1;

  return compareOffset(this, target, start, thisStart, end, thisEnd);
}
```
- example usage
```shell
...
if (arguments.length === 0) return utf8Slice(this, 0, length)
return slowToString.apply(this, arguments)
}

Buffer.prototype.equals = function equals (b) {
if (!Buffer.isBuffer(b)) throw new TypeError('Argument must be a Buffer')
if (this === b) return true
return Buffer.compare(this, b) === 0
}

Buffer.prototype.inspect = function inspect () {
var str = ''
var max = exports.INSPECT_MAX_BYTES
if (this.length > 0) {
  str = this.toString('hex', 0, max).match(/.{2}/g).join(' ')
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.copy"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>copy ()](#apidoc.element.socket.io-stream.Buffer.prototype.copy)
- description and source-code
```javascript
function copy() { [native code] }
```
- example usage
```shell
...
  if (len > value.byteLength - offset) {
    throw new RangeError('\'length\' is out of bounds');
  }
  return new Buffer(value.slice(offset, offset + len));
}
if (Buffer.isBuffer(value)) {
  var out = new Buffer(value.length);
  value.copy(out, 0, 0, value.length);
  return out;
}
if (value) {
  if (Array.isArray(value) || (typeof ArrayBuffer !== 'undefined' && value.buffer instanceof ArrayBuffer) || 'length' in value) {
    return new Buffer(value);
  }
  if (value.type === 'Buffer' && Array.isArray(value.data)) {
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.equals"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>equals (b)](#apidoc.element.socket.io-stream.Buffer.prototype.equals)
- description and source-code
```javascript
function equals(b) {
  if (!(b instanceof Buffer))
    throw new TypeError('Argument must be a Buffer');

  if (this === b)
    return true;

  return binding.compare(this, b) === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.fill"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>fill (val, start, end, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.fill)
- description and source-code
```javascript
function fill(val, start, end, encoding) {
  // Handle string cases:
  if (typeof val === 'string') {
    if (typeof start === 'string') {
      encoding = start;
      start = 0;
      end = this.length;
    } else if (typeof end === 'string') {
      encoding = end;
      end = this.length;
    }

    if (encoding !== undefined && typeof encoding !== 'string') {
      throw new TypeError('encoding must be a string');
    }
    var normalizedEncoding = internalUtil.normalizeEncoding(encoding);
    if (normalizedEncoding === undefined) {
      throw new TypeError('Unknown encoding: ' + encoding);
    }

    if (val.length === 0) {
      // Previously, if val === '', the Buffer would not fill,
      // which is rather surprising.
      val = 0;
    } else if (val.length === 1) {
      var code = val.charCodeAt(0);
      if ((normalizedEncoding === 'utf8' && code < 128) ||
          normalizedEncoding === 'latin1') {
        // Fast path: If 'val' fits into a single byte, use that numeric value.
        val = code;
      }
    }
  } else if (typeof val === 'number') {
    val = val & 255;
  }

  // Invalid ranges are not set to a default, so can range check early.
  if (start < 0 || end > this.length)
    throw new RangeError('Out of range index');

  if (end <= start)
    return this;

  start = start >>> 0;
  end = end === undefined ? this.length : end >>> 0;

  binding.fill(this, val, start, end, encoding);

  return this;
}
```
- example usage
```shell
...
  var fillBuf = new Buffer(_fill, enc);
  var flen = fillBuf.length;
  var i = -1;
  while (++i < size) {
    buf[i] = fillBuf[i % flen];
  }
} else {
  buf.fill(_fill);
}
return buf;
}
exports.allocUnsafe = function allocUnsafe(size) {
if (typeof Buffer.allocUnsafe === 'function') {
  return Buffer.allocUnsafe(size);
}
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.hexSlice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>hexSlice ()](#apidoc.element.socket.io-stream.Buffer.prototype.hexSlice)
- description and source-code
```javascript
function hexSlice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.hexWrite"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>hexWrite ()](#apidoc.element.socket.io-stream.Buffer.prototype.hexWrite)
- description and source-code
```javascript
function hexWrite() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.includes"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>includes (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.includes)
- description and source-code
```javascript
function includes(val, byteOffset, encoding) {
  return this.indexOf(val, byteOffset, encoding) !== -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.indexOf"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>indexOf (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.indexOf)
- description and source-code
```javascript
function indexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, true);
}
```
- example usage
```shell
...
/**
 * Emits streams to this corresponding server/client.
 *
 * @return {Socket} self
 * @api public
 */
Socket.prototype.emit = function(type) {
  if (~exports.events.indexOf(type)) {
    return emit.apply(this, arguments);
  }
  this._stream.apply(this, arguments);
  return this;
};

Socket.prototype.on = function(type, listener) {
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.inspect"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>inspect ()](#apidoc.element.socket.io-stream.Buffer.prototype.inspect)
- description and source-code
```javascript
function inspect() {
  var str = '';
  var max = exports.INSPECT_MAX_BYTES;
  if (this.length > 0) {
    str = this.toString('hex', 0, max).match(/.{2}/g).join(' ');
    if (this.length > max)
      str += ' ... ';
  }
  return '<' + this.constructor.name + ' ' + str + '>';
}
```
- example usage
```shell
...
if (ctx.customInspect &&
    value &&
    isFunction(value.inspect) &&
    // Filter out the util module, it's inspect function is special
    value.inspect !== exports.inspect &&
    // Also filter out any prototype objects using the circular check.
    !(value.constructor && value.constructor.prototype === value)) {
  var ret = value.inspect(recurseTimes, ctx);
  if (!isString(ret)) {
    ret = formatValue(ctx, ret, recurseTimes);
  }
  return ret;
}

// Primitive types cannot have properties
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.lastIndexOf"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>lastIndexOf (val, byteOffset, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.lastIndexOf)
- description and source-code
```javascript
function lastIndexOf(val, byteOffset, encoding) {
  return bidirectionalIndexOf(this, val, byteOffset, encoding, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.latin1Slice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>latin1Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.latin1Slice)
- description and source-code
```javascript
function latin1Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.latin1Write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>latin1Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.latin1Write)
- description and source-code
```javascript
function latin1Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readDoubleBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readDoubleBE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readDoubleBE)
- description and source-code
```javascript
function readDoubleBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readDoubleLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readDoubleLE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readDoubleLE)
- description and source-code
```javascript
function readDoubleLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 8, this.length);
  return binding.readDoubleLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readFloatBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readFloatBE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readFloatBE)
- description and source-code
```javascript
function readFloatBE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatBE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readFloatLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readFloatLE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readFloatLE)
- description and source-code
```javascript
function readFloatLE(offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);
  return binding.readFloatLE(this, offset);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readInt16BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt16BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt16BE)
- description and source-code
```javascript
readInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset + 1] | (this[offset] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readInt16LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt16LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt16LE)
- description and source-code
```javascript
readInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  var val = this[offset] | (this[offset + 1] << 8);
  return (val & 0x8000) ? val | 0xFFFF0000 : val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readInt32BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt32BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt32BE)
- description and source-code
```javascript
readInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] << 24) |
      (this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      (this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readInt32LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt32LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt32LE)
- description and source-code
```javascript
readInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16) |
      (this[offset + 3] << 24);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readInt8"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readInt8 (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readInt8)
- description and source-code
```javascript
readInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  var val = this[offset];
  return !(val & 0x80) ? val : (0xff - val + 1) * -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readIntBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readIntBE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readIntBE)
- description and source-code
```javascript
readIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var i = byteLength;
  var mul = 1;
  var val = this[offset + --i];
  while (i > 0 && (mul *= 0x100))
    val += this[offset + --i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readIntLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readIntLE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readIntLE)
- description and source-code
```javascript
readIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;
  mul *= 0x80;

  if (val >= mul)
    val -= Math.pow(2, 8 * byteLength);

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUInt16BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt16BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt16BE)
- description and source-code
```javascript
readUInt16BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return (this[offset] << 8) | this[offset + 1];
}
```
- example usage
```shell
...
  }
}

function read (buf, i) {
  if (indexSize === 1) {
    return buf[i]
  } else {
    return buf.readUInt16BE(i * indexSize)
  }
}

var i
if (dir) {
  var foundIndex = -1
  for (i = byteOffset; i < arrLength; i++) {
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUInt16LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt16LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt16LE)
- description and source-code
```javascript
readUInt16LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 2, this.length);
  return this[offset] | (this[offset + 1] << 8);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUInt32BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt32BE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt32BE)
- description and source-code
```javascript
readUInt32BE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return (this[offset] * 0x1000000) +
      ((this[offset + 1] << 16) |
      (this[offset + 2] << 8) |
      this[offset + 3]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUInt32LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt32LE (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt32LE)
- description and source-code
```javascript
readUInt32LE = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 4, this.length);

  return ((this[offset]) |
      (this[offset + 1] << 8) |
      (this[offset + 2] << 16)) +
      (this[offset + 3] * 0x1000000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUInt8"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUInt8 (offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUInt8)
- description and source-code
```javascript
readUInt8 = function (offset, noAssert) {
  offset = offset >>> 0;
  if (!noAssert)
    checkOffset(offset, 1, this.length);
  return this[offset];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUIntBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUIntBE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUIntBE)
- description and source-code
```javascript
readUIntBE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset + --byteLength];
  var mul = 1;
  while (byteLength > 0 && (mul *= 0x100))
    val += this[offset + --byteLength] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.readUIntLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>readUIntLE (offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.readUIntLE)
- description and source-code
```javascript
readUIntLE = function (offset, byteLength, noAssert) {
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert)
    checkOffset(offset, byteLength, this.length);

  var val = this[offset];
  var mul = 1;
  var i = 0;
  while (++i < byteLength && (mul *= 0x100))
    val += this[offset + i] * mul;

  return val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.slice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>slice (start, end)](#apidoc.element.socket.io-stream.Buffer.prototype.slice)
- description and source-code
```javascript
function slice(start, end) {
  const srcLength = this.length;
  start = adjustOffset(start, srcLength);
  end = end !== undefined ? adjustOffset(end, srcLength) : srcLength;
  const newLength = end > start ? end - start : 0;
  return new FastBuffer(this.buffer, this.byteOffset + start, newLength);
}
```
- example usage
```shell
...
  }
  if (offset >= value.byteLength) {
    throw new RangeError('\'offset\' is out of bounds');
  }
  if (len > value.byteLength - offset) {
    throw new RangeError('\'length\' is out of bounds');
  }
  return new Buffer(value.slice(offset, offset + len));
}
if (Buffer.isBuffer(value)) {
  var out = new Buffer(value.length);
  value.copy(out, 0, 0, value.length);
  return out;
}
if (value) {
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.swap16"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap16 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap16)
- description and source-code
```javascript
function swap16() {
  // For Buffer.length < 128, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 2 !== 0)
    throw new RangeError('Buffer size must be a multiple of 16-bits');
  if (len < 128) {
    for (var i = 0; i < len; i += 2)
      swap(this, i, i + 1);
    return this;
  }
  return swap16n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.swap32"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap32 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap32)
- description and source-code
```javascript
function swap32() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 4 !== 0)
    throw new RangeError('Buffer size must be a multiple of 32-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 4) {
      swap(this, i, i + 3);
      swap(this, i + 1, i + 2);
    }
    return this;
  }
  return swap32n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.swap64"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>swap64 ()](#apidoc.element.socket.io-stream.Buffer.prototype.swap64)
- description and source-code
```javascript
function swap64() {
  // For Buffer.length < 192, it's generally faster to
  // do the swap in javascript. For larger buffers,
  // dropping down to the native code is faster.
  const len = this.length;
  if (len % 8 !== 0)
    throw new RangeError('Buffer size must be a multiple of 64-bits');
  if (len < 192) {
    for (var i = 0; i < len; i += 8) {
      swap(this, i, i + 7);
      swap(this, i + 1, i + 6);
      swap(this, i + 2, i + 5);
      swap(this, i + 3, i + 4);
    }
    return this;
  }
  return swap64n(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>toJSON ()](#apidoc.element.socket.io-stream.Buffer.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.length) {
    const data = [];
    for (var i = 0; i < this.length; ++i)
      data[i] = this[i];
    return { type: 'Buffer', data };
  } else {
    return { type: 'Buffer', data: [] };
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.toString"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>toString ()](#apidoc.element.socket.io-stream.Buffer.prototype.toString)
- description and source-code
```javascript
toString = function () {
  let result;
  if (arguments.length === 0) {
    result = this.utf8Slice(0, this.length);
  } else {
    result = slowToString.apply(this, arguments);
  }
  if (result === undefined)
    throw new Error('"toString()" failed');
  return result;
}
```
- example usage
```shell
...
){
return a           // if the placeholder was passed, return
  ? (              // a random number from 0 to 15
    a ^            // unless b is 8,
    Math.random()  // in which case
    * 16           // a random number from
    >> a/4         // 8 to 11
    ).toString(16) // in hexadecimal
  : (              // or otherwise a concatenated string:
    [1e7] +        // 10000000 +
    -1e3 +         // -1000 +
    -4e3 +         // -4000 +
    -8e3 +         // -80000000 +
    -1e11          // -100000000000,
    ).replace(     // replacing
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.ucs2Slice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>ucs2Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.ucs2Slice)
- description and source-code
```javascript
function ucs2Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.ucs2Write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>ucs2Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.ucs2Write)
- description and source-code
```javascript
function ucs2Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.utf8Slice"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>utf8Slice ()](#apidoc.element.socket.io-stream.Buffer.prototype.utf8Slice)
- description and source-code
```javascript
function utf8Slice() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.utf8Write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>utf8Write ()](#apidoc.element.socket.io-stream.Buffer.prototype.utf8Write)
- description and source-code
```javascript
function utf8Write() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>write (string, offset, length, encoding)](#apidoc.element.socket.io-stream.Buffer.prototype.write)
- description and source-code
```javascript
write = function (string, offset, length, encoding) {
  // Buffer#write(string);
  if (offset === undefined) {
    encoding = 'utf8';
    length = this.length;
    offset = 0;

  // Buffer#write(string, encoding)
  } else if (length === undefined && typeof offset === 'string') {
    encoding = offset;
    length = this.length;
    offset = 0;

  // Buffer#write(string, offset[, length][, encoding])
  } else if (isFinite(offset)) {
    offset = offset >>> 0;
    if (isFinite(length)) {
      length = length >>> 0;
      if (encoding === undefined)
        encoding = 'utf8';
    } else {
      encoding = length;
      length = undefined;
    }
  } else {
    // if someone is still calling the obsolete form of write(), tell them.
    // we don't want eg buf.write("foo", "utf8", 10) to silently turn into
    // buf.write("foo", "utf8"), so we can't ignore extra args
    throw new Error('Buffer.write(string, encoding, offset[, length]) ' +
                    'is no longer supported');
  }

  var remaining = this.length - offset;
  if (length === undefined || length > remaining)
    length = remaining;

  if (string.length > 0 && (length < 0 || offset < 0))
    throw new RangeError('Attempt to write outside buffer bounds');

  if (!encoding)
    encoding = 'utf8';

  var loweredCase = false;
  for (;;) {
    switch (encoding) {
      case 'hex':
        return this.hexWrite(string, offset, length);

      case 'utf8':
      case 'utf-8':
        return this.utf8Write(string, offset, length);

      case 'ascii':
        return this.asciiWrite(string, offset, length);

      case 'latin1':
      case 'binary':
        return this.latin1Write(string, offset, length);

      case 'base64':
        // Warning: maxLength not taken into account in base64Write
        return this.base64Write(string, offset, length);

      case 'ucs2':
      case 'ucs-2':
      case 'utf16le':
      case 'utf-16le':
        return this.ucs2Write(string, offset, length);

      default:
        if (loweredCase)
          throw new TypeError('Unknown encoding: ' + encoding);
        encoding = ('' + encoding).toLowerCase();
        loweredCase = true;
    }
  }
}
```
- example usage
```shell
...

### ss.Buffer

[Node Buffer](https://nodejs.org/api/buffer.html) class to use on browser, which is exposed for convenience. On Node environment
, you should just use normal 'Buffer'.

'''js
var stream = ss.createStream();
stream.write(new ss.Buffer([0, 1, 2]));
'''

## License

MIT
...
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeDoubleBE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleBE)
- description and source-code
```javascript
function writeDoubleBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleBE(this, val, offset);
  else
    binding.writeDoubleBE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeDoubleLE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeDoubleLE)
- description and source-code
```javascript
function writeDoubleLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeDoubleLE(this, val, offset);
  else
    binding.writeDoubleLE(this, val, offset, true);
  return offset + 8;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeFloatBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeFloatBE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeFloatBE)
- description and source-code
```javascript
function writeFloatBE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatBE(this, val, offset);
  else
    binding.writeFloatBE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeFloatLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeFloatLE (val, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeFloatLE)
- description and source-code
```javascript
function writeFloatLE(val, offset, noAssert) {
  val = +val;
  offset = offset >>> 0;
  if (!noAssert)
    binding.writeFloatLE(this, val, offset);
  else
    binding.writeFloatLE(this, val, offset, true);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeInt16BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt16BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt16BE)
- description and source-code
```javascript
writeInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeInt16LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt16LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt16LE)
- description and source-code
```javascript
writeInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0x7fff, -0x8000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeInt32BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt32BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt32BE)
- description and source-code
```javascript
writeInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeInt32LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt32LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt32LE)
- description and source-code
```javascript
writeInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0x7fffffff, -0x80000000);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  this[offset + 2] = (value >>> 16);
  this[offset + 3] = (value >>> 24);
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeInt8"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeInt8 (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeInt8)
- description and source-code
```javascript
writeInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0x7f, -0x80);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeIntBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeIntBE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeIntBE)
- description and source-code
```javascript
writeIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = byteLength - 1;
  var mul = 1;
  var sub = 0;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i + 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeIntLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeIntLE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeIntLE)
- description and source-code
```javascript
writeIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert) {
    checkInt(this,
             value,
             offset,
             byteLength,
             Math.pow(2, 8 * byteLength - 1) - 1,
             -Math.pow(2, 8 * byteLength - 1));
  }

  var i = 0;
  var mul = 1;
  var sub = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100)) {
    if (value < 0 && sub === 0 && this[offset + i - 1] !== 0)
      sub = 1;
    this[offset + i] = ((value / mul) >> 0) - sub;
  }

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt16BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16BE)
- description and source-code
```javascript
writeUInt16BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = (value >>> 8);
  this[offset + 1] = value;
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt16LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt16LE)
- description and source-code
```javascript
writeUInt16LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 2, 0xffff, 0);
  this[offset] = value;
  this[offset + 1] = (value >>> 8);
  return offset + 2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32BE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt32BE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32BE)
- description and source-code
```javascript
writeUInt32BE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset] = (value >>> 24);
  this[offset + 1] = (value >>> 16);
  this[offset + 2] = (value >>> 8);
  this[offset + 3] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32LE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt32LE (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt32LE)
- description and source-code
```javascript
writeUInt32LE = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 4, 0xffffffff, 0);
  this[offset + 3] = (value >>> 24);
  this[offset + 2] = (value >>> 16);
  this[offset + 1] = (value >>> 8);
  this[offset] = value;
  return offset + 4;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUInt8"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUInt8 (value, offset, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUInt8)
- description and source-code
```javascript
writeUInt8 = function (value, offset, noAssert) {
  value = +value;
  offset = offset >>> 0;
  if (!noAssert)
    checkInt(this, value, offset, 1, 0xff, 0);
  this[offset] = value;
  return offset + 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUIntBE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUIntBE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUIntBE)
- description and source-code
```javascript
writeUIntBE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var i = byteLength - 1;
  var mul = 1;
  this[offset + i] = value;
  while (--i >= 0 && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Buffer.prototype.writeUIntLE"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Buffer.prototype.</span>writeUIntLE (value, offset, byteLength, noAssert)](#apidoc.element.socket.io-stream.Buffer.prototype.writeUIntLE)
- description and source-code
```javascript
writeUIntLE = function (value, offset, byteLength, noAssert) {
  value = +value;
  offset = offset >>> 0;
  byteLength = byteLength >>> 0;
  if (!noAssert) {
    const maxBytes = Math.pow(2, 8 * byteLength) - 1;
    checkInt(this, value, offset, byteLength, maxBytes, 0);
  }

  var mul = 1;
  var i = 0;
  this[offset] = value;
  while (++i < byteLength && (mul *= 0x100))
    this[offset + i] = (value / mul) >>> 0;

  return offset + byteLength;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io-stream.IOStream"></a>[module socket.io-stream.IOStream](#apidoc.module.socket.io-stream.IOStream)

#### <a name="apidoc.element.socket.io-stream.IOStream.IOStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.IOStream.IOStream)
- description and source-code
```javascript
function IOStream(options) {
  if (!(this instanceof IOStream)) {
    return new IOStream(options);
  }

  IOStream.super_.call(this, options);

  this.options = options;
  this.id = uuid();
  this.socket = null;

  // Buffers
  this.pushBuffer = [];
  this.writeBuffer = [];

  // Op states
  this._readable = false;
  this._writable = false;
  this.destroyed = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  this.on('finish', this._onfinish);
  this.on('end', this._onend);
  this.on('error', this._onerror);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.IOStream.super_"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.</span>super_ (options)](#apidoc.element.socket.io-stream.IOStream.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io-stream.IOStream.prototype"></a>[module socket.io-stream.IOStream.prototype](#apidoc.module.socket.io-stream.IOStream.prototype)

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._done"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_done ()](#apidoc.element.socket.io-stream.IOStream.prototype._done)
- description and source-code
```javascript
_done = function () {
  this._readable = false;

  // signal the end of the data.
  return this.push(null);
}
```
- example usage
```shell
...
* @api private
*/
IOStream.prototype._end = function() {
 if (this.pushBuffer.length) {
   // end after flushing buffer.
   this.pushBuffer.push(bind(this, '_done'));
 } else {
   this._done();
 }
};

/**
* Remote stream just ended
*
* @api private
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._end"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_end ()](#apidoc.element.socket.io-stream.IOStream.prototype._end)
- description and source-code
```javascript
_end = function () {
  if (this.pushBuffer.length) {
    // end after flushing buffer.
    this.pushBuffer.push(bind(this, '_done'));
  } else {
    this._done();
  }
}
```
- example usage
```shell
...
 * @api private
 */
IOStream.prototype._onfinish = function() {
debug('_onfinish');
// Local socket just finished
// send 'end' event to remote
if (this.socket) {
  this.socket._end(this.id);
}

this.writable = false;
this._writableState.ended = true;

if (!this.readable || this._readableState.ended) {
  debug('_onfinish: ended, destroy %s', this._readableState);
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._onend"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onend ()](#apidoc.element.socket.io-stream.IOStream.prototype._onend)
- description and source-code
```javascript
_onend = function () {
  debug('_onend');
  this.readable = false;
  this._readableState.ended = true;

  if (!this.writable || this._writableState.finished) {
    debug('_onend: %s', this._writableState);
    return this.destroy();
  }

  debug('_onend: not finished');

  if (!this.allowHalfOpen) {
    this.end();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._onerror"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onerror (err)](#apidoc.element.socket.io-stream.IOStream.prototype._onerror)
- description and source-code
```javascript
_onerror = function (err) {
  // check if the error came from remote stream.
  if (!err.remote && this.socket) {
    // notify the error to the corresponding remote stream.
    this.socket._error(this.id, err);
  }

  this.destroy();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._onfinish"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onfinish ()](#apidoc.element.socket.io-stream.IOStream.prototype._onfinish)
- description and source-code
```javascript
_onfinish = function () {
  debug('_onfinish');
  // Local socket just finished
  // send 'end' event to remote
  if (this.socket) {
    this.socket._end(this.id);
  }

  this.writable = false;
  this._writableState.ended = true;

  if (!this.readable || this._readableState.ended) {
    debug('_onfinish: ended, destroy %s', this._readableState);
    return this.destroy();
  }

  debug('_onfinish: not ended');

  if (!this.allowHalfOpen) {
    this.push(null);

    // just in case we're waiting for an EOF.
    if (this.readable && !this._readableState.endEmitted) {
      this.read(0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._onread"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onread (size)](#apidoc.element.socket.io-stream.IOStream.prototype._onread)
- description and source-code
```javascript
_onread = function (size) {
  var write = this.writeBuffer.shift();
  if (write) return write();

  this._writable = true;
}
```
- example usage
```shell
...
};

Socket.prototype._onread = function(id, size) {
debug('read: "%s"', id);

var stream = this.streams[id];
if (stream) {
  stream._onread(size);
} else {
  debug('ignore invalid stream id');
}
};

Socket.prototype._onwrite = function(id, chunk, encoding, callback) {
debug('write: "%s"', id);
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._onwrite"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_onwrite (chunk, encoding, callback)](#apidoc.element.socket.io-stream.IOStream.prototype._onwrite)
- description and source-code
```javascript
_onwrite = function (chunk, encoding, callback) {
  var self = this;

  function push() {
    self._readable = false;
    var ret = self.push(chunk || '', encoding);
    callback();
    return ret;
  }

  if (this._readable) {
    push();
  } else {
    this.pushBuffer.push(push);
  }
}
```
- example usage
```shell
...
  return;
}

if (global.ArrayBuffer && chunk instanceof ArrayBuffer) {
  // make sure that chunk is a buffer for stream
  chunk = new Buffer(new Uint8Array(chunk));
}
stream._onwrite(chunk, encoding, callback);
};

Socket.prototype._onend = function(id) {
debug('end: "%s"', id);

var stream = this.streams[id];
if (!stream) {
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._read"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_read (size)](#apidoc.element.socket.io-stream.IOStream.prototype._read)
- description and source-code
```javascript
_read = function (size) {
  var push;

  // We can not read from the socket if it's destroyed obviously ...
  if (this.destroyed) return;

  if (this.pushBuffer.length) {
    // flush buffer and end if it exists.
    while (push = this.pushBuffer.shift()) {
      if (!push()) break;
    }
    return;
  }

  this._readable = true;

  // Go get data from remote stream
  // Calls
  // ._onread remotely
  // then
  // ._onwrite locally
  this.socket._read(this.id, size);
}
```
- example usage
```shell
...
 this._readable = true;

 // Go get data from remote stream
 // Calls
 // ._onread remotely
 // then
 // ._onwrite locally
 this.socket._read(this.id, size);
};


/**
* Read from remote stream
*
* @api private
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype._write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>_write (chunk, encoding, callback)](#apidoc.element.socket.io-stream.IOStream.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, callback) {
  var self = this;

  function write() {
    // We can not write to the socket if it's destroyed obviously ...
    if (self.destroyed) return;

    self._writable = false;
    self.socket._write(self.id, chunk, encoding, callback);
  }

  if (this._writable) {
    write();
  } else {
    this.writeBuffer.push(write);
  }
}
```
- example usage
```shell
...
var self = this;

function write() {
  // We can not write to the socket if it's destroyed obviously ...
  if (self.destroyed) return;

  self._writable = false;
  self.socket._write(self.id, chunk, encoding, callback);
}

if (this._writable) {
  write();
} else {
  this.writeBuffer.push(write);
}
...
```

#### <a name="apidoc.element.socket.io-stream.IOStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">socket.io-stream.IOStream.prototype.</span>destroy ()](#apidoc.element.socket.io-stream.IOStream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  debug('destroy');

  if (this.destroyed) {
    debug('already destroyed');
    return;
  }

  this.readable = this.writable = false;

  if (this.socket) {
    debug('clean up');
    this.socket.cleanup(this.id);
    this.socket = null;
  }

  this.destroyed = true;
}
```
- example usage
```shell
...
}

this.writable = false;
this._writableState.ended = true;

if (!this.readable || this._readableState.ended) {
  debug('_onfinish: ended, destroy %s', this._readableState);
  return this.destroy();
}

debug('_onfinish: not ended');

if (!this.allowHalfOpen) {
  this.push(null);
...
```



# <a name="apidoc.module.socket.io-stream.Socket"></a>[module socket.io-stream.Socket](#apidoc.module.socket.io-stream.Socket)

#### <a name="apidoc.element.socket.io-stream.Socket.Socket"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.Socket.Socket)
- description and source-code
```javascript
function Socket(sio, options) {
  if (!(this instanceof Socket)) {
    return new Socket(sio, options);
  }

  EventEmitter.call(this);

  options = options || {};

  this.sio = sio;
  this.forceBase64 = !!options.forceBase64;
  this.streams = {};
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();

  var eventName = exports.event;
  sio.on(eventName, bind(this, emit));
  sio.on(eventName + '-read', bind(this, '_onread'));
  sio.on(eventName + '-write', bind(this, '_onwrite'));
  sio.on(eventName + '-end', bind(this, '_onend'));
  sio.on(eventName + '-error', bind(this, '_onerror'));
  sio.on('error', bind(this, emit, 'error'));
  sio.on('disconnect', bind(this, '_ondisconnect'));

  this.encoder.on('stream', bind(this, '_onencode'));
  this.decoder.on('stream', bind(this, '_ondecode'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.super_"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.</span>super_ ()](#apidoc.element.socket.io-stream.Socket.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io-stream.Socket.prototype"></a>[module socket.io-stream.Socket.prototype](#apidoc.module.socket.io-stream.Socket.prototype)

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._end"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_end (id)](#apidoc.element.socket.io-stream.Socket.prototype._end)
- description and source-code
```javascript
_end = function (id) {
  this.sio.emit(exports.event + '-end', id);
}
```
- example usage
```shell
...
 * @api private
 */
IOStream.prototype._onfinish = function() {
debug('_onfinish');
// Local socket just finished
// send 'end' event to remote
if (this.socket) {
  this.socket._end(this.id);
}

this.writable = false;
this._writableState.ended = true;

if (!this.readable || this._readableState.ended) {
  debug('_onfinish: ended, destroy %s', this._readableState);
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._error"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_error (id, err)](#apidoc.element.socket.io-stream.Socket.prototype._error)
- description and source-code
```javascript
_error = function (id, err) {
  this.sio.emit(exports.event + '-error', id, err.message || err);
}
```
- example usage
```shell
...
 *
 * @api private
 */
IOStream.prototype._onerror = function(err) {
  // check if the error came from remote stream.
  if (!err.remote && this.socket) {
    // notify the error to the corresponding remote stream.
    this.socket._error(this.id, err);
  }

  this.destroy();
};

},{"./uuid":7,"component-bind":12,"debug":14,"stream":35,"util":40}],5:[function(require,module,exports){
var util = require('util');
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._ondecode"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_ondecode (stream)](#apidoc.element.socket.io-stream.Socket.prototype._ondecode)
- description and source-code
```javascript
_ondecode = function (stream) {
  var id = stream.id;
  if (this.streams[id]) {
    this._error(id, new Error('Decoded stream already exists: ' + id));
    return;
  }

  this.streams[id] = stream;
  stream.socket = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._ondisconnect"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_ondisconnect ()](#apidoc.element.socket.io-stream.Socket.prototype._ondisconnect)
- description and source-code
```javascript
_ondisconnect = function () {
  var stream;
  for (var id in this.streams) {
    stream = this.streams[id];
    stream.destroy();

    // Close streams when the underlaying
    // socket.io connection is closed (regardless why)
    stream.emit('close');
    stream.emit('error', new Error('Connection aborted'));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onencode"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onencode (stream)](#apidoc.element.socket.io-stream.Socket.prototype._onencode)
- description and source-code
```javascript
_onencode = function (stream) {
  if (stream.socket || stream.destroyed) {
    throw new Error('stream has already been sent.');
  }

  var id = stream.id;
  if (this.streams[id]) {
    throw new Error('Encoded stream already exists: ' + id);
  }

  this.streams[id] = stream;
  stream.socket = this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onend"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onend (id)](#apidoc.element.socket.io-stream.Socket.prototype._onend)
- description and source-code
```javascript
_onend = function (id) {
  debug('end: "%s"', id);

  var stream = this.streams[id];
  if (!stream) {
    debug('ignore non-existent stream id: "%s"', id);
    return;
  }

  stream._end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onerror"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onerror (id, message)](#apidoc.element.socket.io-stream.Socket.prototype._onerror)
- description and source-code
```javascript
_onerror = function (id, message) {
  debug('error: "%s", "%s"', id, message);

  var stream = this.streams[id];
  if (!stream) {
    debug('invalid stream id: "%s"', id);
    return;
  }

  var err = new Error(message);
  err.remote = true;
  stream.emit('error', err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onread"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onread (id, size)](#apidoc.element.socket.io-stream.Socket.prototype._onread)
- description and source-code
```javascript
_onread = function (id, size) {
  debug('read: "%s"', id);

  var stream = this.streams[id];
  if (stream) {
    stream._onread(size);
  } else {
    debug('ignore invalid stream id');
  }
}
```
- example usage
```shell
...
};

Socket.prototype._onread = function(id, size) {
debug('read: "%s"', id);

var stream = this.streams[id];
if (stream) {
  stream._onread(size);
} else {
  debug('ignore invalid stream id');
}
};

Socket.prototype._onwrite = function(id, chunk, encoding, callback) {
debug('write: "%s"', id);
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onstream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onstream (type, listener)](#apidoc.element.socket.io-stream.Socket.prototype._onstream)
- description and source-code
```javascript
_onstream = function (type, listener) {
  if ('function' != typeof listener) {
    throw TypeError('listener must be a function');
  }

  function onstream() {
    debug('new streams');
    var self = this;
    var args = slice.call(arguments);
    var ack = args[args.length - 1];
    if ('function' == typeof ack) {
      args[args.length - 1] = function() {
        var args = slice.call(arguments);
        args = self.encoder.encode(args);
        ack.apply(this, args);
      };
    }

    args = this.decoder.decode(args);
    listener.apply(this, args);
  }

  // for removeListener
  onstream.listener = listener;

  on.call(this, type, onstream);
}
```
- example usage
```shell
...
};

Socket.prototype.on = function(type, listener) {
 if (~exports.events.indexOf(type)) {
   return on.apply(this, arguments);
 }

 this._onstream(type, listener);
 return this;
};

/**
* Sends a new stream request.
*
* @param {String} event type
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._onwrite"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_onwrite (id, chunk, encoding, callback)](#apidoc.element.socket.io-stream.Socket.prototype._onwrite)
- description and source-code
```javascript
_onwrite = function (id, chunk, encoding, callback) {
  debug('write: "%s"', id);

  var stream = this.streams[id];
  if (!stream) {
    callback('invalid stream id: ' + id);
    return;
  }

  if (global.ArrayBuffer && chunk instanceof ArrayBuffer) {
    // make sure that chunk is a buffer for stream
    chunk = new Buffer(new Uint8Array(chunk));
  }
  stream._onwrite(chunk, encoding, callback);
}
```
- example usage
```shell
...
  return;
}

if (global.ArrayBuffer && chunk instanceof ArrayBuffer) {
  // make sure that chunk is a buffer for stream
  chunk = new Buffer(new Uint8Array(chunk));
}
stream._onwrite(chunk, encoding, callback);
};

Socket.prototype._onend = function(id) {
debug('end: "%s"', id);

var stream = this.streams[id];
if (!stream) {
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._read"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_read (id, size)](#apidoc.element.socket.io-stream.Socket.prototype._read)
- description and source-code
```javascript
_read = function (id, size) {
  this.sio.emit(exports.event + '-read', id, size);
}
```
- example usage
```shell
...
 this._readable = true;

 // Go get data from remote stream
 // Calls
 // ._onread remotely
 // then
 // ._onwrite locally
 this.socket._read(this.id, size);
};


/**
* Read from remote stream
*
* @api private
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._stream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_stream (type)](#apidoc.element.socket.io-stream.Socket.prototype._stream)
- description and source-code
```javascript
_stream = function (type) {
  debug('sending new streams');

  var self = this;
  var args = slice.call(arguments, 1);
  var ack = args[args.length - 1];
  if ('function' == typeof ack) {
    args[args.length - 1] = function() {
      var args = slice.call(arguments);
      args = self.decoder.decode(args);
      ack.apply(this, args);
    };
  }

  args = this.encoder.encode(args);
  var sio = this.sio;
  sio.emit.apply(sio, [exports.event, type].concat(args));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype._write"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>_write (id, chunk, encoding, callback)](#apidoc.element.socket.io-stream.Socket.prototype._write)
- description and source-code
```javascript
_write = function (id, chunk, encoding, callback) {
  if (Buffer.isBuffer(chunk)) {
    if (this.forceBase64) {
      encoding = 'base64';
      chunk = chunk.toString(encoding);
    } else if (!global.Buffer) {
      // socket.io can't handle Buffer when using browserify.
      if (chunk.toArrayBuffer) {
        chunk = chunk.toArrayBuffer();
      } else {
        chunk = chunk.buffer;
      }
    }
  }
  this.sio.emit(exports.event + '-write', id, chunk, encoding, callback);
}
```
- example usage
```shell
...
var self = this;

function write() {
  // We can not write to the socket if it's destroyed obviously ...
  if (self.destroyed) return;

  self._writable = false;
  self.socket._write(self.id, chunk, encoding, callback);
}

if (this._writable) {
  write();
} else {
  this.writeBuffer.push(write);
}
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype.cleanup"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>cleanup (id)](#apidoc.element.socket.io-stream.Socket.prototype.cleanup)
- description and source-code
```javascript
cleanup = function (id) {
  delete this.streams[id];
}
```
- example usage
```shell
...
    return;
  }

  this.readable = this.writable = false;

  if (this.socket) {
    debug('clean up');
    this.socket.cleanup(this.id);
    this.socket = null;
  }

  this.destroyed = true;
};

/**
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype.emit"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>emit (type)](#apidoc.element.socket.io-stream.Socket.prototype.emit)
- description and source-code
```javascript
emit = function (type) {
  if (~exports.events.indexOf(type)) {
    return emit.apply(this, arguments);
  }
  this._stream.apply(this, arguments);
  return this;
}
```
- example usage
```shell
...
var io = require('socket.io-client');
var ss = require('socket.io-stream');

var socket = io.connect('http://example.com/user');
var stream = ss.createStream();
var filename = 'profile.jpg';

ss(socket).emit('profile-image', stream, {name: filename});
fs.createReadStream(filename).pipe(stream);
'''

You can stream data from a client to server, and vice versa.

'''js
// send data
...
```

#### <a name="apidoc.element.socket.io-stream.Socket.prototype.on"></a>[function <span class="apidocSignatureSpan">socket.io-stream.Socket.prototype.</span>on (type, listener)](#apidoc.element.socket.io-stream.Socket.prototype.on)
- description and source-code
```javascript
on = function (type, listener) {
  if (~exports.events.indexOf(type)) {
    return on.apply(this, arguments);
  }

  this._onstream(type, listener);
  return this;
}
```
- example usage
```shell
...
Server:

'''js
var io = require('socket.io').listen(80);
var ss = require('socket.io-stream');
var path = require('path');

io.of('/user').on('connection', function(socket) {
  ss(socket).on('profile-image', function(stream, data) {
    var filename = path.basename(data.name);
    stream.pipe(fs.createWriteStream(filename));
  });
});
'''
...
```



# <a name="apidoc.module.socket.io-stream.blob_read_stream"></a>[module socket.io-stream.blob_read_stream](#apidoc.module.socket.io-stream.blob_read_stream)

#### <a name="apidoc.element.socket.io-stream.blob_read_stream.blob_read_stream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>blob_read_stream (blob, options)](#apidoc.element.socket.io-stream.blob_read_stream.blob_read_stream)
- description and source-code
```javascript
function BlobReadStream(blob, options) {
  if (!(this instanceof BlobReadStream)) {
    return new BlobReadStream(blob, options);
  }

  Readable.call(this, options);

  options = options || {};
  this.blob = blob;
  this.slice = blob.slice || blob.webkitSlice || blob.mozSlice;
  this.start = 0;
  this.sync = options.synchronous || false;

  var fileReader;

  if (options.synchronous) {
    fileReader = this.fileReader = new FileReaderSync();
  } else {
    fileReader = this.fileReader = new FileReader();
  }

  fileReader.onload = bind(this, '_onload');
  fileReader.onerror = bind(this, '_onerror');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.blob_read_stream.super_"></a>[function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.</span>super_ (options)](#apidoc.element.socket.io-stream.blob_read_stream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io-stream.blob_read_stream.prototype"></a>[module socket.io-stream.blob_read_stream.prototype](#apidoc.module.socket.io-stream.blob_read_stream.prototype)

#### <a name="apidoc.element.socket.io-stream.blob_read_stream.prototype._onerror"></a>[function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_onerror (e)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._onerror)
- description and source-code
```javascript
_onerror = function (e) {
  var err = e.target.error;
  this.emit('error', err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.blob_read_stream.prototype._onload"></a>[function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_onload (e)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._onload)
- description and source-code
```javascript
_onload = function (e) {
  var chunk = new Buffer(new Uint8Array(e.target.result));
  this.push(chunk);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.blob_read_stream.prototype._read"></a>[function <span class="apidocSignatureSpan">socket.io-stream.blob_read_stream.prototype.</span>_read (size)](#apidoc.element.socket.io-stream.blob_read_stream.prototype._read)
- description and source-code
```javascript
_read = function (size) {
  var start = this.start;
  var end = this.start = this.start + size;
  var chunk = this.slice.call(this.blob, start, end);

  if (chunk.size) {
    if (this.sync) {
      var bufferChunk = new Buffer(new Uint8Array(this.fileReader.readAsArrayBuffer(chunk)));
      this.push(bufferChunk);
    } else {
      this.fileReader.readAsArrayBuffer(chunk);
    }
  } else {
    this.push(null);
  }
}
```
- example usage
```shell
...
 this._readable = true;

 // Go get data from remote stream
 // Calls
 // ._onread remotely
 // then
 // ._onwrite locally
 this.socket._read(this.id, size);
};


/**
* Read from remote stream
*
* @api private
...
```



# <a name="apidoc.module.socket.io-stream.parser"></a>[module socket.io-stream.parser](#apidoc.module.socket.io-stream.parser)

#### <a name="apidoc.element.socket.io-stream.parser.Decoder"></a>[function <span class="apidocSignatureSpan">socket.io-stream.parser.</span>Decoder ()](#apidoc.element.socket.io-stream.parser.Decoder)
- description and source-code
```javascript
function Decoder() {
  EventEmitter.call(this);
}
```
- example usage
```shell
...

options = options || {};

this.sio = sio;
this.forceBase64 = !!options.forceBase64;
this.streams = {};
this.encoder = new parser.Encoder();
this.decoder = new parser.Decoder();

var eventName = exports.event;
sio.on(eventName, bind(this, emit));
sio.on(eventName + '-read', bind(this, '_onread'));
sio.on(eventName + '-write', bind(this, '_onwrite'));
sio.on(eventName + '-end', bind(this, '_onend'));
sio.on(eventName + '-error', bind(this, '_onerror'));
...
```

#### <a name="apidoc.element.socket.io-stream.parser.Encoder"></a>[function <span class="apidocSignatureSpan">socket.io-stream.parser.</span>Encoder ()](#apidoc.element.socket.io-stream.parser.Encoder)
- description and source-code
```javascript
function Encoder() {
  EventEmitter.call(this);
}
```
- example usage
```shell
...
EventEmitter.call(this);

options = options || {};

this.sio = sio;
this.forceBase64 = !!options.forceBase64;
this.streams = {};
this.encoder = new parser.Encoder();
this.decoder = new parser.Decoder();

var eventName = exports.event;
sio.on(eventName, bind(this, emit));
sio.on(eventName + '-read', bind(this, '_onread'));
sio.on(eventName + '-write', bind(this, '_onwrite'));
sio.on(eventName + '-end', bind(this, '_onend'));
...
```



# <a name="apidoc.module.socket.io-stream.socket_io_stream"></a>[module socket.io-stream.socket_io_stream](#apidoc.module.socket.io-stream.socket_io_stream)

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.socket_io_stream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.</span>socket_io_stream (sio, options)](#apidoc.element.socket.io-stream.socket_io_stream.socket_io_stream)
- description and source-code
```javascript
function lookup(sio, options) {
  options = options || {};
  if (null == options.forceBase64) {
    options.forceBase64 = exports.forceBase64;
  }

  if (!sio._streamSocket) {
    sio._streamSocket = new Socket(sio, options);
  }
  return sio._streamSocket;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.Buffer"></a>[function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>Buffer (arg, encodingOrOffset, length)](#apidoc.element.socket.io-stream.socket_io_stream.Buffer)
- description and source-code
```javascript
function Buffer(arg, encodingOrOffset, length) {
  if (!Buffer.TYPED_ARRAY_SUPPORT && !(this instanceof Buffer)) {
    return new Buffer(arg, encodingOrOffset, length)
  }

  // Common case.
  if (typeof arg === 'number') {
    if (typeof encodingOrOffset === 'string') {
      throw new Error(
        'If encoding is specified then the first argument must be a string'
      )
    }
    return allocUnsafe(this, arg)
  }
  return from(this, arg, encodingOrOffset, length)
}
```
- example usage
```shell
...

### ss.Buffer

[Node Buffer](https://nodejs.org/api/buffer.html) class to use on browser, which is exposed for convenience. On Node environment
, you should just use normal 'Buffer'.

'''js
var stream = ss.createStream();
stream.write(new ss.Buffer([0, 1, 2]));
'''

## License

MIT
...
```

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.IOStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>IOStream (options)](#apidoc.element.socket.io-stream.socket_io_stream.IOStream)
- description and source-code
```javascript
function IOStream(options) {
  if (!(this instanceof IOStream)) {
    return new IOStream(options);
  }

  IOStream.super_.call(this, options);

  this.options = options;
  this.id = uuid();
  this.socket = null;

  // Buffers
  this.pushBuffer = [];
  this.writeBuffer = [];

  // Op states
  this._readable = false;
  this._writable = false;
  this.destroyed = false;

  // default to *not* allowing half open sockets
  this.allowHalfOpen = options && options.allowHalfOpen || false;

  this.on('finish', this._onfinish);
  this.on('end', this._onend);
  this.on('error', this._onerror);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.Socket"></a>[function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>Socket (sio, options)](#apidoc.element.socket.io-stream.socket_io_stream.Socket)
- description and source-code
```javascript
function Socket(sio, options) {
  if (!(this instanceof Socket)) {
    return new Socket(sio, options);
  }

  EventEmitter.call(this);

  options = options || {};

  this.sio = sio;
  this.forceBase64 = !!options.forceBase64;
  this.streams = {};
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();

  var eventName = exports.event;
  sio.on(eventName, bind(this, emit));
  sio.on(eventName + '-read', bind(this, '_onread'));
  sio.on(eventName + '-write', bind(this, '_onwrite'));
  sio.on(eventName + '-end', bind(this, '_onend'));
  sio.on(eventName + '-error', bind(this, '_onerror'));
  sio.on('error', bind(this, emit, 'error'));
  sio.on('disconnect', bind(this, '_ondisconnect'));

  this.encoder.on('stream', bind(this, '_onencode'));
  this.decoder.on('stream', bind(this, '_ondecode'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.createBlobReadStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>createBlobReadStream (blob, options)](#apidoc.element.socket.io-stream.socket_io_stream.createBlobReadStream)
- description and source-code
```javascript
createBlobReadStream = function (blob, options) {
  return new BlobReadStream(blob, options);
}
```
- example usage
```shell
...

  $('#file').change(function(e) {
    var file = e.target.files[0];
    var stream = ss.createStream();

    // upload a file to the server.
    ss(socket).emit('file', stream, {size: file.size});
    ss.createBlobReadStream(file).pipe(stream);
  });
});
</script>
'''

#### Upload progress
...
```

#### <a name="apidoc.element.socket.io-stream.socket_io_stream.createStream"></a>[function <span class="apidocSignatureSpan">socket.io-stream.socket_io_stream.</span>createStream (options)](#apidoc.element.socket.io-stream.socket_io_stream.createStream)
- description and source-code
```javascript
createStream = function (options) {
  return new IOStream(options);
}
```
- example usage
```shell
...
Client:

'''js
var io = require('socket.io-client');
var ss = require('socket.io-stream');

var socket = io.connect('http://example.com/user');
var stream = ss.createStream();
var filename = 'profile.jpg';

ss(socket).emit('profile-image', stream, {name: filename});
fs.createReadStream(filename).pipe(stream);
'''

You can stream data from a client to server, and vice versa.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
