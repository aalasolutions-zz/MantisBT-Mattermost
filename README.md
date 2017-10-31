MantisBT-Mattermost
==============

A [MantisBT](http://www.mantisbt.org/) plugin to send bug updates to [Mattermost](https://about.mattermost.com/) 
channels.

It is only for Mantis 2.0.x, not backward compatible.


# Setup
1. Extract this repo to your *Mantis folder/plugins/Mattermost*.
2. On Mattermost, add a new "Incoming Webhooks" for your channel and note the URL that Mattermost generates 
for you.
3. On the MantisBT side, access the plugin's configuration page and fill in your Mattermost webhook URL.
4. You can map your MantisBT projects to Mattermost channels by setting the *plugin_Matter_channels* option in 
Mantis.  
5. Follow the instructions on the plugin's configuration page to get there. Make sure the *plugin_Matter_channels* 
configuration option is set to "All Users", with type "complex". Example value for this setting:


          array (
              'Mantis Project Name as Appear With Spaces' => 'general',
              'My Other Short Named Mantis Project' => 'second-project'
          )


6. You can specify which bug fields appear in the Matter notifications. Edit the *plugin_Matter_columns* configuration 
option for this purpose.  Follow the instructions on the plugin configuration page.
