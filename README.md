Crypter
=======

A small app written in Java for drag and drop file encryption.
It uses 128bit AES encryption with passsword.
Maximum file size supported is 20 MB.
Command line support is achieved using jArgs (http://jargs.sourceforge.net/) command line option parsing suite for Java

ChangeLog:
==========
Added command line support. Files can be encrypted from the command line/terminal.

Added execcutable jar. Check inside the jar folder

Command line parameters:
========================

For encryption : -e or --encrypt
For decryption : -d or --decrypt
Either -e or -d should be specified.

To specify password : -p password (required)



Examples:
=========

java -jar crypter.jar -e -p mypassword file1.ext file2.ext file3.ext 

java -jar crypter.jar -d -p mypassword file1.ext.enc file2.ext.enc

In the above examples, "mypassword" is the password

You can switch the encryption and password arguments. The only requirement is that list of files should be specified at the end.
