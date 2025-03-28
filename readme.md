# Thunder and Lightning

Early in my days of building Halloween props, I mostly just bookmarked projects that other people did so I could replicate them. I had the idea to have thunder sounds play over speakers while timed in sync with triggering a strobe light to generate a lightning effect. I've played with video editing software, so I knew there was probably some way to accurately time the lightning crackling sound with turning on a strobe light.

The more I poked around the Internet, I came across an [Instructables LightshowPi](https://www.instructables.com/Raspberry-Pi-LightshowPi/) link that showed how to use a Raspberry Pi to play Christmas music and it would time strings of lights to play along - somewhat auto-magically. I was intrigued thinking that instead of Christmas music, I'd have a playlist of different thunder sound effects and just trigger a strobe light instead.

The more I read, and the more I learned - I figured the effect would be better produced if I triggered three separate bright white flood lights that were scattered across the yard. Instead of one strobe light just getting turned on and off, I could have the lightning "ripple" across the yard. The LightshowPi software "listens" to the sound files and tries to guess when to trigger the GPIO pins (which in turn trigger a relay switch).

## Parts list
- Raspberry Pi - any model, even the older ones are more than sufficient
- [Relay module](https://www.sainsmart.com/products/8-channel-5v-relay-module) to interface between Raspberry Pi and standard 3 prong electrical cord.
- Three [flood light stakes](https://www.homedepot.com/p/Commercial-Electric-CE-Metal-Lamp-Holder-LPHR-01/309407190) and bright white flood lights
- [LightshowPi software](https://www.lightshowpi.org/)
- Three short three prong extension cords to cut and connect female end to relay board

Installation and configuration of the LightshowPi software was super simple. Wiring the relay board just meant connecting trigger GPIO pins to the input pins on the board, plus 5V and ground. Make sure the jumper on the relay board is on the VCC side (and not JD-VCC). Wiring the extension cord ends was a little tricky. The wire gauge thickness for the plugs was a bit thick in the relay jacks. They tend to pull out very easily. Next, connect speakers to the Raspberry Pi, then start the software. I had it automatically play a playlist of seven different thunder and lightning mp3 files, and it auto-magically synced the three flood lights based on the audio. It was very effective as a low cost prop.

![Wiring diagram](/assets/wiring diagram.jpg)
![Working build](/assets/setup.JPG)
