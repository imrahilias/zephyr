# new approach
1) chrome oe1.orf.at
2) inspect
3) in inspect window crtl f > search 'mp3' > loopstream(...).mp3
4) open link in new tab
5) download

# rip mp3 stream on 7tage oe1
https://bitcointalk.org/index.php?topic=29451.0
google: [OT] Tip + Frage: Webradio speichern?

# howto
start iceweasel (install addblock plus)
run site (oe1.orf.at > 7tage) & click play on the flash plugin
iceweasel > tools > addblock plus > open blockable items
find loopstream adress (http://loopstream01.apa.at/*') in the list of blockable content
vlc open media > convert/save (ctr+r) > network > paste addr, select mp3 (or flac), etc
convert/save

# old, doesnt work anymore / temporary
##console > $ mplayer -dumpstream -dumpfile /path/to/dir/foobar.mp3 'streamadress'

# example
## loopstream: http://loopstream01.apa.at/?channel=oe1&shoutcast=0&ua=flash&id=20130406_2303_54_1_jazznacht_JAN_m_
## mplayer -dumpstream -dumpfile ~/jazznacht_130407.mp3 'http://loopstream01.apa.at/?channel=oe1&shoutcast=0&ua=flash&id=20130406_2303_54_1_jazznacht_JAN_m_'

# live stream mp3 stats
http://mp3stream3.apasf.apa.at:8000/listen.pls

mplayer spricht beim rippen von:
     Name   : OE 1
     Genre  : Classic
     Website: http://oe1.orf.at
     Public : yes
     Bitrate: 120kbit/s

Allerdings sagt mplayer (und vlc) beim abspielen:
AUDIO: 44100 Hz, 2 ch, floatle, 80.0 kbit/2.83% (ratio: 10000->352800)

# live stream wma stats
mms://apasf.apa.at/oe1_live_worldwide

Allerdings sagt mplayer beim abspielen:
AUDIO: 44100 Hz, 2 ch, s16le, 64.0 kbit/4.54% (ratio: 8003->176400)

Vlc hingegen:
Windows Media Audio 2 (wma2), 44100 Hz, 2 ch, 16bit


# mp3 > wma