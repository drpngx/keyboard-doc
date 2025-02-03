# Svalboard initial setup
This document records my first impressions of my Svalboard setup. It also serves as
typing practice.

It is addressed to prospective and new Svalboard users out there. My experience will
be different from yours. You should probably try different options.

## Fitment
The great misconception that held me back was that the keys had to be perpendicular to the
the fingers. Not so.

### When you got it wrong
Initially, it was so bad that I thought that my unit had been shipped with debouncing
accidentally turned off. I would press keys and it would repeat the same key many, many
times.

I positioned my thumb all the way up so that my nail would press on the top of the nail
key, which does not trigger the key reliably.

### Homing position
It took me a day to figure this out. This is the way it works for me to get reliable
key presses and initially positioning my hand without bumping into keys.

The position of the thumb is right at where the key moves down. Five millimeters below
and it will not move down.

The other digits are resting on the corner of three keys, towards the center. This means
that the presses on these keys are going to be a little between side press and press down.
The presses on the other keys are going to be extensions outward. So you have mostly two
finger movement classes to manage. The down movement is more natural. The out movement
is the tricky one and I find that it doesn't accidentally trigger multiple keys this way.

If you look at the default layout, you will find that the West keys on the left hand and
the East keys on the right hand have been assigned to less frequently used symbols.

I changed the yaw so that the keys angle gently downward. It also minimizes travel to the
out side key.

When you position your hands that way, it feels a little like you are lower on the keyboard.
This is like resting your hand on the `ZXCV` row of a normal keyboard. There is no corresponding
clutching movement to reach for a lower row. It feels a little unnatural at first.

So, to be clear, the resting position of the fingers are:
* left pinky: down south east
* left annular: down south east
* left middle: down south
* left index: down south west
* right index: down south east
* right middle: down south
* right annular: down south west
* right pinky: down south west

Once you have your fingers in that position, you rotate your palm until the thumb is
grazing both the pad and knuckle keys.

This is the position that minimizes accidental typos for me, and I believe it's also the
config that was intended. Strange that it took me so long to figure out.

### Notes
The most surprinsing is that the thumb rotation is quite limited. Even if you move the palm
rest out of the way it appears to be limited below.

Space is limited and for those who have small hands like me the clusters will touch each other
and compete for space. They are ok for now but during exploration I felt that I could have used
an extra millimeter or so.

I found that keys would stop working when they were too close and I had to move or rotate them
slightly to make them work.

## Layout design
It is a highly subjective topic, so I'm going to explain my decisions and you can act accordingly.

### Constraints
Unlike regular keyboards, effort is light and there is no shift in hand position while typing.
On a regular keyboard, when you press the thumb, you may have to rotate your hand slightly
or move it up. That limits the combinations that you can achieve comfortably with the same
hand. On the Svalboard, I find that there is no such constraint. So, if you have control
on the right or left thumb makes no difference to how you design the layout of the other digits.

Digits of the same hand tend to move together. So, if you have a modifier on the East key
of your right annular, be aware that the combination with, say, the West key of your right
middle finger will be more awkward and slower to type. As a rule I have modifiers on both
sides and I use them to trigger the opposite hand.

#### Thumb clusters
The thumbs can press only one key at a time, except the fat finger combos:
* knuckle-nail: e.g. control tab on the default left thumb
* pad-mode: this is possible but somewhat awkward

For now I'm going to imagine that they don't exist. I find them awkward anyway.

It's clear that the nail and mode keys can only be used for tap and not modifiers.

The best keys for modifiers are, in order of decreasing preference: down, pad, knuckle.

### Prime real-estate
When you assign keys, you will find that some keys are easier to press than others.
To the extent possible, you'll want keep reserve them for modifier keys, keys that
you type often such as space or backspace.

I'm going to give you a point system. I haven't used it myself but I want to express
how difficult it is to press some keys, so that prospective buyers can make a determination
for themselves. Higher means better.

Fingers:
* Right hand: `+5`
* Thumb: `+100`
* Index: `+40`
* Middle: `+50`
* Ring: `+20`
* Pinky: `0`
* Digit down: `+20`
* Digit south: `+15`
* Digit up: `+8`
* Left digit east or right digit west: `+5`
* Left digit west or right digit east: `-5`
* Thumb down: `+50`
* Thumb pad: `+30`
* Thumb knuckle: `+15`
* Thumb nail: `0`
* Thumb up: `-10`

### Before you do anything else: Pads get a thumb down
There is one decision you need to make a priori before anything else, and it's hard to revert afterwards.
It's what you put on the thumb down. They are the most valuable real estate in the entire keyboard.

The big fight is for the right thumb down: should it get a layer modifier or space?

If you anticipate spending a lot of time holding key to access a second layer, then use that.
From my usage patterns, I like to type fast more than I spend time in another layer. So, I use space.

As an emacs user, I use control a lot and I considered putting control as the pad key, and enter on the
knuckle instead. The only reason I kept the current config is to see if I would use the control tab combo.

### Base layer
I keep the default QWERTY. I tried changing a while back but emacs was all messed up.

### Layer styles
I considered three options:
* using modal layers: a layer toggle, then it's sticky (`TO`), or sticky once (`OSM`). For the toggle, it means
  that you have to spend another key going back to the base layer. It's good design to reserve that key on all
  layers, so that means you need two layer keys or more. Mostly, modal (stateful) keyboards are not for me.
* using a spacious two layer system: you use two layers, perhaps one for digits and one for navigation.
  That also means you need two layer keys. That is what I have on my Iris CE because of the fact that, once
  you press down one thumb, then there are de facto only two rows that are usable on the same hand. So there
  is one layer for each thumb. The Svalboard has no such constraint. You could use the thumb down keys for
  layer activation and shift on the other layer, swapping them in the layer.
* using a single upper layer accessible through a modifier: this is what I picked. It is packed but so far it
  appears to work.

### Modifier keys
As an Emacs user, you need them everywhere. You want them on the thumb to minimize strain, but also on
the vermicular fingers. Each thumb can only press one modifier at a time so you need them on other fingers
too.

#### Mod-taps
It is my experience that you can't type your fastest with mod-taps. It will easily shave 10 WPM and introduce
annoying display latency. Plus, misfires can trigger weird actions. I have opened a new browser tab by accident
more than once.

But I think they are a necessary evil. I find that they can be used on keys that don't need as much speed. So,
they can be attached to keys that are not space or letters. During coding, some key combinations need to be
fast, such as `C-x`, `C-c`, `C-d`, and the navigation keys. Since the arrow keys are readily available,
I use those more often now.

To facilitate learning, it's best if they be on the same location on all layers. It facilitates typing when
you activate a layer: you don't have to think in which order you pressed the layer or modifier key. Unfortuntely,
the only available spots on the base layer are "outer" keys on the fingers which are not ideal. I have changed
them to the down key on the up layers where available, but I kept the outer ones.

The index finger on the base layer has letters in all directions so it can't be used. The stronger fingers use
the most useful modifiers. So it's:
* Shift for middle finger
* Control for ring finger
* Alt for pinky

### Cardinality
For the upper layer, I pay attention to geometry and cardinality. Essentially, there are four keygroups
that I need to fit:
* Numbers: they are 10, so they don't fit neatly in a row of eight fingers. So I use two thumb clusters.
  Digits of lower ordinality are used more frequently so they get the stronger keys: `1` down, `2` south,
  etc
* Function keys: same thing. They are used less frequently but I still put them on the right hand is where
  my layer key is
* Arrow keys: they get the right index finger which is not the strongest but the most agile. Also, I didn't
  want to split my function clusters
* Pagination keys: home, end, page up, page down.

Once I made the decision not to spread horizontally, going finger by finger fit nicely. If you type numbers
all day long, this might not work best for you.

### One-handed operation
Quite common among gamers, the right hand moves the mouse while the left hand can do limited tasks.
Sometimes I use my cell phone with one hand.
Things like alt-tab would be nice. Unfortunately this config is not one hand compatible.

### Sanity check
I'll be using the Emacs notation here:
* `C` means control,
* `S` means shift,
* `s` means super aka Windows key,
* `M` means meta aka ALT.

Once you have a layout, it's useful to mentally check that you can still type less frequently
use but nonetheless useful combinations that you like.

Windows and Chrome:
* `C-S-<tab>`
* `s-r`: run command
* `C-S-ESC`: taskmgr
* `C-M-<f4>`: close window. It's important that you can type this comfortably because if it
  goes into repeat mode it could be bad. Ask me how I know.
* `C-<end>`
* `M-<tab>` pressed down while using arrow keys (I use `s-<tab>` instead, which is sticky
* `C-M-<left>`: browser back
* your frequently-used passwords

Emacs:
* `C-_`: undo
* `M-^`: join line
* `M-%`: replace string
* keychords. For instance I use `cv` for `M-x recompile`.
Some new combinations opened up such as `M-}` which was previously awkward.
Emacs can always be configured, of course, but if you remap too many keys, ask yourself
the question if the problem is in the layout.

## Emacs

### Keyboard minor mode
Unlike other keyboards that I have learned, the Svalboard will take more
than a day to learn. This day 3 and I am still at 30 wpm without punctuation
versus `100+` wpm on my Iris CE with punctuation. I'll take a while to get
to a point where I can use the Svalboard as my single primary keyboard.

During that time, I need to be able to switch between keyboards. Most of my
key bindings will remain the same but navigation keys will change from `vi`-style
to directions.

In the Iris CE, I have the function keys on two rows on top of each other, whereas
on the Svalboard, they occupy two finger clusters.

I use these keys for directional navigation and to quick jump to shells, of which
I have `10`.

On the Iris CE, I use `<f1>` through `<f5>` to quick jump to shells. Because the
middle row is so valuable, I use that to navigate between buffers using the
`vi`-style directions. So, `<f6>` is `windmove-left`, `<f7>` down, etc. To access
the shells `6` and above I use `C-<f6>` for shell `6` etc.

On the Svalboard, moving to shells is just `C-<fX>` to move to shell `X`. For
navigation, I use the `<f1>` to `<f5>` cluster.

In Emacs, switching the keymaps and modeline is a pain so I'll just use two
minor modes. First we define the keymaps:
```
(defvar drpng-keymap-iris (make-sparse-keymap) "Keymap for Iris CE.")
(defvar drpng-keymap-sval (make-sparse-keymap) "Keymap for Svalboard.")

(define-key drpng-keymap-iris (png-kbd "<f6>") 'buf-nav-move-or-kill-left)
(define-key drpng-keymap-iris (png-kbd "<f9>") 'buf-nav-move-or-kill-right)
(define-key drpng-keymap-iris (png-kbd "<f8>") 'buf-nav-move-or-kill-up)
(define-key drpng-keymap-iris (png-kbd "<f7>") 'buf-nav-move-or-kill-down)
(define-key drpng-keymap-iris (png-kbd "<f1>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 1)))
(define-key drpng-keymap-iris (png-kbd "<f2>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 2)))
(define-key drpng-keymap-iris (png-kbd "<f3>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 3)))
(define-key drpng-keymap-iris (png-kbd "<f4>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 4)))
(define-key drpng-keymap-iris (png-kbd "<f5>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 5)))
(define-key drpng-keymap-iris (png-kbd "C-<f1>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 6)))
(define-key drpng-keymap-iris (png-kbd "C-<f2>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 7)))
(define-key drpng-keymap-iris (png-kbd "C-<f3>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 8)))
(define-key drpng-keymap-iris (png-kbd "C-<f4>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 9)))
(define-key drpng-keymap-iris (png-kbd "C-<f5>")
            (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 10)))

;; Svalboard
(define-key drpng-keymap-sval (png-kbd "<f5>") 'buf-nav-move-or-kill-left)
(define-key drpng-keymap-sval (png-kbd "<f3>") 'buf-nav-move-or-kill-right)
(define-key drpng-keymap-sval (png-kbd "<f4>") 'buf-nav-move-or-kill-up)
(define-key drpng-keymap-sval (png-kbd "<f2>") 'buf-nav-move-or-kill-down)
(define-key drpng-keymap-sval (png-kbd "C-<f1>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 1)))
(define-key drpng-keymap-sval (png-kbd "C-<f2>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 2)))
(define-key drpng-keymap-sval (png-kbd "C-<f3>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 3)))
(define-key drpng-keymap-sval (png-kbd "C-<f4>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 4)))
(define-key drpng-keymap-sval (png-kbd "C-<f5>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 5)))
(define-key drpng-keymap-sval (png-kbd "C-<f6>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 6)))
(define-key drpng-keymap-sval (png-kbd "C-<f7>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 7)))
(define-key drpng-keymap-sval (png-kbd "C-<f8>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 8)))
(define-key drpng-keymap-sval (png-kbd "C-<f9>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 9)))
(define-key drpng-keymap-sval (png-kbd "C-<f10>")
                (lambda () (interactive) (buf-nav-find-or-create-shell-buffer 10)))
```
Then, we can define the minor modes and define the layout switching function.
```

(define-minor-mode drpng-keyboard-layout-iris-mode
  "The keybindings for the Iris CE keyboard."
  :global t
  :lighter " Iris"
  :keymap drpng-keymap-iris)

(define-minor-mode drpng-keyboard-layout-sval-mode
  "The keybindings for the Svalboard keyboard."
  :global t
  :lighter " Sval"
  :keymap drpng-keymap-sval)

(drpng-keyboard-layout-iris-mode 1)

(defun drpng-switch-keymap ()
  "Switch keymaps."
  (interactive)
  (let* ((choices '(("Iris CE" . iris)
                    ("Svalboard" . sval)))
         (selection (completing-read "Select keyboard: " (mapcar #'car choices) nil t))
         (selected-mode (cdr (assoc selection choices))))
    (if (eq selected-mode 'iris)
        (progn
          (drpng-keyboard-layout-iris-mode 1)
          (drpng-keyboard-layout-sval-mode 0))
      (drpng-keyboard-layout-iris-mode 0)
      (drpng-keyboard-layout-sval-mode 1))
    (message "Switched to %s" selection)))
```
