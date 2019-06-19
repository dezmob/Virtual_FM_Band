> Check out the real-life [GTA: San Andreas radio set](https://raphaelyancey.fr/projects/grand-theft-auto-san-andreas-radio-set.html) for an example use of this library

# Virtual_FM_Band

A virtual FM band playing simultaneous sounds over virtual frequencies.

```
                                                                        
Track 0        Track 1        Track 2        Track 3       Track N        
   |              |              |              |             |         
   |--------------|--------------|--------------|---- - - - --|         
                                                                        
   <------------------------------------------------- - - - -->         
                         virtual frequency                     
                                                                        
```

Technically, it's a mixer with multiple tracks that takes care of the volume of each track (fade in / fade out) while moving along the virtual frequency.

## Installation

In the project root:
* `brew install portaudio mad` (OSX) or `apt-get install libportaudio0 libportaudio2 libportaudiocpp0 libmad0-dev portaudio19-dev libasound-dev` (Debian)
* `pip install virtualenv` (if not already installed on your machine)
* `virtualenv --python=python2.7` (or whatever Python 2 binary you've got)
* `source bin/activate`
* `pip install -r requirements.txt`

## TODO
  - [ ] Move all variables in an .env file
  - [ ] Handle streams as input
  - [ ] Add static noise between stations
  - [ ] Make swmixer play the files in loop
  - [ ] Do not play if the file is not to be heard anyway
  - [ ] Random start position
