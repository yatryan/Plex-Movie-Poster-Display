# Plex Movie Poster Display
Scraps the Plex sessions page to display the current playing movie or TV show poster on a screen.

Disclaimer – I am a network engineer not a programmer. I play around with code. I am publishing this to give back to the communities that has helped me learn. There may be better ways of scraping the Plex Posters, but this is the way I chose to do it. I am open to suggestions. Use at your own risk.

I decided to rewrite the program in PHP and make it browser based. This allows me to have the Raspberry Pi boot to the desktop, automatically start a browser in kiosk mode, and open the PHP site.

This script scraps http://IP_ADDRESS_OF_PLEX_SERVER>:32400/status/sessions for clients and displays the poster of the currently playing movie or TV show. If nothing is currently playing it will pull a random poster of an unwatched movie.

## My Setup
Plex Media Server is running on a dedicated server.
Plex Movie Poster Display is running on separate Raspberry Pi 3 connected to a screen via HDMI. On boot up the Pi launches Chromium in kiosk mode and loads the Plex Movie Poster Display URL.

## Help
https://www.mattsshack.com/plex-movie-poster-display/
