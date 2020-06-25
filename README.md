# Mopidy-RadioBrowser

Fork of Ralf's excellent radio browser extention. I have built this capability into a Moode compatible install here: https://github.com/duracell80/MoodeRadio-Get and will be looking to bring configuration options developed there to Mopidy such as limiting the tag list to a reasonable length.

Mopidy extension for playing music from http://www.radio-browser.info. Listen to the world’s radio with 28,000+ stations of music, sports and news streaming from every continent. Acknowledgement and thanks to Nick Steel's `TuneIn plugin <https://github.com/kingosticks/mopidy-tunein>`_ that was based on. This product uses RadioBrowser API but is not endorsed, certified or otherwise approved in any way by RadioBrowser.

## Installation

Install by running

    sudo python3 setup.py install

Some radio streams may require additional audio plugins.
These can be found in the gstreamer plugin packages for your system.
See https://mopidy.com/ext/radiobrowser/ for alternative installation methods.


## Configuration

Before starting Mopidy, you must add configuration for Mopidy-RadioBrowser to your Mopidy configuration file.

- NEW: Encoding, choose which codecs you want the API to return
- NEW: Whitelist tags annd countries to cut down on the amount of scrolling in the library
- NEW: Choose to hide the lanuguages category in the library
- NEW: Choose to hide the top rated category in the library
- TODO: Save a last 50 listened to stations in library

```
[radiobrowser]
enabled = true
timeout = 5000
encoding = aac, flac
whitelist_exact = true
whitelist_tags = jazz, ambient, nature
whitelist_countries = united kingdom, united states, ireland, germany, norway
display_languages = true
display_toprated = true
```

sudo reboot

## Project resources

- `Source code <https://github.com/RalfLangeDresden/mopidy-radiobrowser>`_
- `Issue tracker <https://github.com/RalfLangeDresden/mopidy-radiobrowser/issues>`_
- `Changelog <https://github.com/RalfLangeDresden/mopidy-radiobrowser/blob/master/CHANGELOG.rst>`_


Credits

- Original author: `Ralf Lange <https://github.com/RalfLangeDresden>`__
- Current maintainer: `Ralf Lange <https://github.com/RalfLangeDresden>`__
- `Contributors <https://github.com/RalfLangeDresden/mopidy-radiobrowser/graphs/contributors>`_
