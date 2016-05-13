# ipinfo-for-slack

Custom slash command to use find DNS records for a domain. 

## REQUIREMENTS

* A custom slash command on a Slack team
* A web server running PHP5 with cURL enabled
* A valid SSL certificate for your web server (use https://letsencrypt.org/)

## USAGE

* Place the `hostlookuo.php` script on a server running PHP5 with cURL and a valid SSL certificate.
* Set up a new custom slash command on your Slack team: https://slack.com/apps/A0F82E8CA-slash-commands
* Under "Choose a command", enter whatever you want for the command. /hostlookup is easy to remember.
* Under "URL", enter the URL for the script on your server.
* Leave "Method" set to "Post".
* Decide whether you want this command to show in the autocomplete list for slash commands.
* If you do, enter a short description and usage hint.
* Update the `hostlookup.php` script with your slash command's token.

## NOTICE

This is built off of the work of isitup-for-slack. Check out their stuff:
https://github.com/mccreath/isitup-for-slack/
