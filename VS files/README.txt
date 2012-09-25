autoexp.dat is used by the visual studio debugger to display your classes in
a human readable format. For example, the Sportvision class Vec3 is displayed
as 3 separate float values rather than just an array. This file needs to be placed
in C:\Program Files (x86)\Microsoft Visual Studio 10.0\Common7\Packages\Debugger
(or wherever your visual studio is installed) for VS2010.
-------------------------------

StepOver.reg adds definitions to the registry so the debugger no longer steps
into common things like std::vector::operator=, new, and so on - stuff you 
almost never want to step into when you hit F11. 

If you ever do want to step into somethign, you'll have to briefly edit the
Registry. Ya, wonderful design Microsoft.

This works for VS2010. Earlier versions did not use the registry.
See http://blogs.msdn.com/b/andypennell/archive/2004/02/06/69004.aspx
for more details.

PLEASE NOTE that this does not work for VS2012!! the blogged linked 
above hints on how to make it work for VS2012.

