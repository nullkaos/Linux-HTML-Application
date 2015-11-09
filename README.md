# Linux-HTML-Application
A spin off of Windows HTML Application

&nbsp;&nbsp;&nbsp;&nbsp;By combining a small server with a GUI designed using
Python and Gtk glade one gets the core of LHTA. Using the small server one can
execute cgi scripts that can be based off of Bash, Pearl, Python or anything
else considered a scripting language. The only thing currently un-availabe is
using Php. <br>
&nbsp;&nbsp;&nbsp;&nbsp;To change the window frame, simply edit the .glade file
located in the resources directory. Edit between lines 5 through 10 with the
tag <br>  <property name="type_hint">toolbar</property> <br>
Edit the value with one bellow : <br>

Normal = Remove Line 10 Content<br>
Dialog = dialog<br>
Menu = menu<br>
Toolbar = toolbar<br>
Splash Screen = splashscreen<br>
Utility = utility<br>
Dock = dock<br>
Desktop = desktop<br>
Drop Down Menu = dropdown-menu <br>
Popup Menu = popup-menu<br>
Tooltip = tooltip<br>
Notification = notification<br>
Combo = combo<br>
ans lastly <br>
Drag and Drop = dnd<br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;To handle window positioning, simply .glade file
located in the resources directory. Edit between lines 5 through 10 with the tag
<br> <property name="window_position">center</property> <br>
 Edit the value with one bellow : <br>

None = Remove Line 10 Content<br>
Center = center <br>
Mouse = mouse <br>
Always Center = center-always <br>
Center on Parent = center-on-parent <br>
&nbsp;&nbsp;&nbsp;&nbsp;To add an icon simply add or edit between lines 5 - 10
with either : <br>
    <property name="icon_name">application-exit</property> <br>
# OR <br>
     <property name="icon">icon.png</property> <br>
Icon_Name would be the name of a standard system icon. Ie : refresh or play or
stop, etc. Just having Icon means you need to give the path of an icon -
Relative or otherwise.<br>

&nbsp;&nbsp;&nbsp;&nbsp;To allow/disallow resizing simply add or edit between
lines 5 - 10 with either : <br>
<property name="resizable">True</property> <br>
<property name="resizable">False</property> <br>

&nbsp;&nbsp;&nbsp;&nbsp;To allow/disallow deletion of the window from the
window border simply add or edit between lines 5 - 10 with either : <br>
<property name="deletable">True</property> <br>
<property name="deletable">False</property> <br>
Please not you can still kill the program from a script if you so desire.
Please also note it is urged to kill the program from the script as using the
window border will not kill the server.<br>

&nbsp;&nbsp;&nbsp;&nbsp; You can change the server port to anything above 1024.
Simply edit the root directory lgta python file with any text editor and edit
line 27. By default the port is set to 8080. Also edit line 43 to match you new
port number!
