Place these files in ```jamroom/modules/jrHelloWorld```

Once logged in as master admin,
goto: ```http://YOUR-SITE.com/core/cache_reset``` to reset the caches.  If its still not there, run the integrity check ```http://YOUR-SITE.com/core/integrity_check``` .

You should then see your new jrHelloWorld module under the 'site' section of the admin panel.

If its not active already activate it from the info tab ```http://YOUR-SITE.com/hello/admin/info``` .

'Hello World' should now be visible at this location ```http://YOUR-SITE.com/hello/world``` .

With a slightly more complicated version (it uses templates) visible at ```http://YOUR-SITE.com/hello/saturday``` .

#Profile Hello World
YOUR-SITE.com/profilename/hello

#Module Magic View 
YOUR-SITE.com/audio/modulehello
YOUR-SITE.com/blog/modulehello

#ACP Page
YOUR-SITE.com/hello/helloadmin

#Via an event listener
YOUR-SITE.com/core/integrity_check
Creates a javascript alert when viewing the integrity check form
Note: You can switch this off using the config setting

#Via a smarty function
{jrHelloWorld_hi}
With the one optional parameter: 
{jrHelloWorld_hi spelling="wrong"}

#Write Hello World to a log using a form (admin only)
YOUR-SITE.com/hello/writetologform
Form is created by view_jrHelloWorld_writetologform.
Runs view_jrHelloWorld_writetologform_save on save (via ajax).

#Via a tab in the jrEmbed TinyMCE popup
Adds a tab to the popup, inserts a placeholder into the editor text which is replaced with 'Hello World!' when the text is displayed.

Response to [Forum Question](http://www.jamroom.net/phpBB2/viewtopic.php?p=236618)
