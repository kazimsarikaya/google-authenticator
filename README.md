Current google authenticator pam module does not support whitelist remote
hosts. I added whitelist network ip address configuration.

The **whitelist** file is

~~~
~/.google_authenticator.whitelist
~~~

The file should have permissions 600 The file format is consist of line with
format:

~~~
x.x.x.x/y
~~~

For a host ip address the prefix should be 32. File should end with empty line,
otherwise the last line can not be used. 
