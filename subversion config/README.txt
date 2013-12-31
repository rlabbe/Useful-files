
The config file lets you configure subversion. 

I have altered the global-ignores variable so that svn does not 
try to include common things that should not be in subversion, 
like debug/release directories, object files, and so on. You 
may want to tailor for your particular needs. It is mostly for 
Visual Studio generated files. 

It lives in %appdata%\Roaming\subversion\config for Windows.
