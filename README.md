# Beeswax
Beeswax is essentially a Spotify ad muter it will not avoid the ads or skip them instead it will simply mute them.

# Requirements

You will only need the Visual Studio 2022 C++ redistributable:
https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170

# How does this work?

This software essentially works by first finding the name of the Spotify desktop application in the taskbar due to the fact that the name is based on what is playing for example when a song is playing it will be in the format "Artist - SongName" but when an ad plays it will be either "Advertisement" or "AdvertName" so when an ad plays we can find it by seeing if the name has a "-" in it. After we have found the name of the application if there is no "-" we will mute it in volume mixer and unmute when the "-" has returned.

# What's next?

I plan to rewrite this code to provide extra functionality and remove a few bugs which are a bit random.

A few of the features I have planned are:

  - GUI that will show you what it thinks is playing and allow you to add some things to a blacklist as some ads have a "-" (barely any though).
  - A better method of checking the name of the program or choosing how often it is checked
  - The ability to easily close the application (possibly appear in the arrow menu on the taskbar)
