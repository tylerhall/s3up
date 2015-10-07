s3up
=========

s3up is a command line tool to store static content in [Amazon S3](http://aws.amazon.com/s3/) following the best practices of [YSlow](http://developer.yahoo.com/yslow/). Specifically, it's for users who want to use S3 as a content delivery network for their images, style sheets, JavaScript, etc.

For each file it uploads, s3up sets a far future expiration date, gzips the content, and versions the file by combining the filename with a timestamp. Each of these actions are optional and can be controlled via the command line. s3up can also automatically compress your images using Yahoo!'s [Smush.it](http://www.smushit.com/ysmush.it/) web service.

A longer explanation and example usage can be found [here](http://clickontyler.com/blog/2009/02/serving-static-content-on-amazon-s3-with-s3up/).

FEATURES
--------

 * Upload multiple files at once - including directories
 * Automatically append timestamps onto files for versioning
 * Upload a gzipped version of each file
 * Add far future expiration header to each file
 * Losslessly compress your images using Smush.it

INSTALL
-------

Requires PHP5 and php_curl extension.

 * Place s3up in a convenient location and make executable.

You're done!

UPDATES
-------

Code is hosted at GitHub: [http://github.com/tylerhall/s3up](http://github.com/tylerhall/s3up)

LICENSE
-------

The MIT License

Copyright (c) 2009 Tyler Hall <tylerhall AT gmail DOT com>

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
