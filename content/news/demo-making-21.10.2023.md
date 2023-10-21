---
title: "Demo-making 21.10.2023 – Fantasy Computers"
date: 2023-10-04T00:00:00+03:00
draft: false
tags: []
---

[![TIC-80 THRIVE demo](/images/tic-80-thrive.png)](https://tic80.com/play?cart=2807)

### Welcome to DOT demo-making day on Saturday 21.10.2023 at Aalto Design Factory

Join us for another day of making and watching [demos](https://en.wikipedia.org/wiki/Demoscene)! This time, the theme is [fantasy consoles](https://en.wikipedia.org/wiki/Fantasy_video_game_console), which are artificially limited virtual computers aiming to make graphics and audio programming simple and fun. Check out the [TIC-80 example page](http://tic80.com/play?cat=5) to get an idea of what these computers are capable of.

We are also visiting Ryoji Ikeda’s exhibition in Amos Rex at 18:00 on the Friday before – to maximize inspiration. This is completely optional but a highly recommended exhibition. See [the event page](/news/ikeda-20.10.2023/) for more info.

### For who?
Anyone interested in computational art. Basic programming skills are recommended, but you can also team up with someone and ask for parameters to explore. We are aiming to make our events as beginner friendly as possible, but as the theme *fantasy computers* is a bit more technical one, this event might not be the absolutely most approachable with a purely visual or musical background. However, in a sense we are all beginners, so if *fantasy computers* sounds like fun, you are very welcome to join us! :)

### Platforms

- [TIC-80](https://tic80.com) – recommended
- [PICO-8](https://www.lexaloffle.com/pico-8.php) – if you don’t mind the paywall
- [WASM-4](https://wasm4.org/) – for web hipsters
- [Uxn+Varvava](https://100r.co/site/uxn.html) – if you are feeling hardcore.

If you have another similar platform in mind that you would like to make a demo with, feel free to ask us. However, our aim is to keep organizing fairly stream-lined.

See also [below](#some-helpful-links-and-instructions) for some helpful links for getting started.

### Timetable
- 10:00 event starts – for the early birds
- **12:00 opening keynote, inspiration**
- 13:30–15:00 recommended lunch window
- 18:30 submission deadline
- **19:00 demo compo**
- 20:00 networking / discussions
- 22:00 event ends

Like last time, you may attend the whole event, just the demo compo, or something in between. If you want to make a demo, or if you are new, we recommend coming to the keynote.

### Location
Aalto Design Factory

Puumiehenkuja 5A, 02150 Espoo

### Remote participation
Our big picture goal is to learn how to organize remote participation smoothly, but depending on organizer resources, we might do or skip this.

### Instructions

Note that the organizers are only familiar with TIC-80 and Uxn (and not super familiar with these either), so we can't offer much help with other platforms. But you can still come and ask, we can try to help!

#### Some helpful links and instructions

##### TIC-80

- [Download TIC-80](https://github.com/nesbox/TIC-80/releases) – if you don't want to use the web version
- [Step-by-step introduction to TIC-80](https://github.com/nesbox/TIC-80/wiki/A-step-by-step-introduction-to-TIC-80,-Part-1---The-Default-Cart) - [Part 2](https://github.com/nesbox/TIC-80/wiki/A-step-by-step-introduction-to-TIC-80,-Part-2---Workflow) includes instructions for saving and loading your demo
- [TIC-80 documentation](https://github.com/nesbox/TIC-80/wiki)
- [Lua reference](https://www.lua.org/manual/5.4/) if you're using lua (the default scripting language), especially the list of functions at the end
- Advanced: To make 3D things, see the [ttri function](https://github.com/nesbox/TIC-80/wiki/ttri) and [this snippet](https://github.com/nesbox/TIC-80/wiki/Code-examples-and-snippets#ttri-xyz-rotation)

##### Uxn+Varvara
- [Compudanzas Uxn tutorial](https://compudanzas.net/uxn_tutorial.html) – This is intended to be completed in seven days, so it might be a bit tough to go through it in one day. We told you it's hardcore!
- [Uxntal on XXIIVV wiki](https://wiki.xxiivv.com/site/uxntal.html)
- [Varvara device reference](https://wiki.xxiivv.com/site/varvara.html) – drawing, audio, etc.
- [Uxntal opcode reference](https://wiki.xxiivv.com/site/uxntal_reference.html)

#### Submitting your entry

##### TIC-80:
1. Ensure that you have added the following metadata to the header of your demo:
    ```
    -- title: title of your demo
    -- author: your (nick)name
    -- desc: short description of your demo or a message you want to show on the big screen
    ```
    (this is for lua, ask us if you're unsure and using a different language)
1. To hide the cursor, add `poke(0x7FC3F,1,1)` to the beginning of your `TIC()` function
1. Save your demo by running `save yourdemo.tic` in the TIC-80 console
1. Export the `.tic` file:
    - If you are using the **web version**: run `get yourdemo.tic` to download the `.tic` file
    - If you are using the **downloaded version**: run `folder`, which should open your file manager, where you can find `yourdemo.tic`
1. Upload the `.tic` file [here](https://party.dot-ry.fi)

##### UXN

Upload your `.com` (or `.tal`) file [here](https://party.dot-ry.fi)

##### Other platforms

Come talk to us at least an hour before the deadline!

### After the event
Recordings of the demos will be published on [DOT’s YouTube](https://www.youtube.com/@TheDOTry), like [last time](https://www.youtube.com/watch?v=xv6Z9RkWEK4&list=PLmRDkQf8W1WEaT5I-F3BpZ46czsg0L_sY).