tos3
====

This is a very simple app to sync files from local directory to Amazon S3. The reason I choose Java is because it can be run anywhere with a single JAR file.

To compile, compile with Amazon SDK for Java.

Usage
-----

First, create a file called "s3credentials.properties" somewhere and put in:

    accessKey=YOUR_ACCESS_KEY
    secretKey=YOUR_SECRET_KEY

Then, to use it, do something like:

    java -jar tos3.jar <directory> <bucket> <path-to-s3credentials.properties> preview

It will show which files to add, or to remove.

Finally, remove the last word, "preview" to make it sync!