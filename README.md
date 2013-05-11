# [mt-downloader](http://tusharmath.github.io/Multi-threaded-downloader)

This is a multi threaded downloader which is made in nodejs. It is highly configurable and extremely efficient.

## Features
1. Supports virtually unlimited number of threads.
2. Auto selective re-download in case of failure.
3. Supports checksum verification.  
   _(View the config file to see all the ways in which you can configure the application)_


## How to use
1. Install [nodejs](http://nodejs.org/) (skip if already done).
2. Install mt-downloader globally.

   ```bash
   $ npm install -g mt-downloader
   ```

3. Open the config file and set the default _download\_path_ for your downloads. To know where your config file is located just type _mtd_ and search for the _Config:_ key word.

   ```bash
   $ mtd
   ```

4. Start using like this -

   ```bash
   $ mtd -u "http://mirror.switch.ch/ftp/mirror/videolan/vlc/2.0.6/macosx/vlc-2.0.6.dmg"
   ```

   By default it will take the last bit of the url as the file name. In this case the file will be downloaded in the default directory (Specified in config) and will be automatically name 'vlc-2.0.6.dmg'.  

   Alternatively you can pass the name of the file with the _-f_ parameter like this -

   ```bash
   $ mtd -u "http://mirror.switch.ch/ftp/mirror/videolan/vlc/2.0.6/macosx/vlc-2.0.6.dmg" -f "vlc.latest.dmg"
   ```


## Issues or Feature Requests?
   Feel free to create one [here](https://github.com/tusharmath/Multi-threaded-downloader/issues/new)
   
   _I Need help in developing code for this application so please contribute if you can!_