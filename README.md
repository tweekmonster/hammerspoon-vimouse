# Hammerspoon Vi Mouse

Control the mouse with [Hammerspoon][] in a Vim-ish way.


## Install

Download `vimouse.lua` and add it to `~/.hammerspoon`.  In
`~/.hammerspoon/init.lua` add:

```lua
local vimouse = require('vimouse')
vimouse('cmd', 'm')
```

This sets <kbd>⌘-m</kbd> as the key that toggles Vi Mouse mode.


## Usage

```lua
-- h/j/k/l moves the mouse cursor by 20 pixels.  Holding shift moves by 100
-- pixels, and holding alt moves by 5 pixels.
--
-- Pressing <space> sends left mouse down.  Releasing <space> sends left mouse
-- up.  Holding <space> and pressing h/j/k/l is mouse dragging.  Tapping
-- <space> quickly sends double and triple clicks.  Holding ctrl sends right
-- mouse events.
--
-- <c-y> and <c-e> sends the scroll wheel event.  Holding the keys will speed
-- up the scrolling.
--
-- Press <esc> or the configured toggle key to end Vi Mouse mode.
```

[Hammerspoon]: http://www.hammerspoon.org/
