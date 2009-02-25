s3up is a command line tool to store static content in [Amazon S3](http://aws.amazon.com/s3/) following the best practices of [YSlow](http://developer.yahoo.com/yslow/). Specifically, it's for users who want to use S3 as a content delivery network for their images, style sheets, JavaScript, etc.

For each file it uploads, s3up sets a far future expiration date, gzips the content, and versions the file by combining the filename with a timestamp. Each of these actions are optional and can be controlled via the command line.

A longer explanation and example usage can be found [here](http://clickontyler.com/blog/2009/02/serving-static-content-on-amazon-s3-with-s3up/).

License
-------

This code is released under the MIT Open Source License. Feel free to do whatever you want with it.
