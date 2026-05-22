---
title: mpf both (command-line utility)
---

# mpf both (command-line utility)


Starts both the MPF game engine and the MPF Media Controller from a
single command window with a single command. This is effectively the
same as running both `mpf game` and `mpf mc`, but more convenient.

When you run `mpf both`, the console log outputs from both MPF and
MPF-MC will be mingled together in the console window. However the log
files in your machine's `/logs` folder will still be separate.

Also note that you can pass command line options to both MPF and MPF-MC
after the "both" command, like this:

``` shell
mpf both -v

mpf both -v -V -b

mpf both -g path/to/godot/project/folder -G ~/path/to/Godot_v4.6-stable_linux.x86_64
```

### -g
Used in MPF 0.80 and beyond. Specifies the Godot project folder, that is the folder where you gmc.cfg file is located.

```
-g path/to/godot/project/folder

```

Typically used together with the -G switch.

### -G

Used in MPF 0.80 and beyond to specify where the Godot editor executable is being located. This is not the executable of your complete Godot setup you can export from Godot editor, but the executable of the Godot editor itself. E.g.

```
-G ~/path/to/Godot_v4.6-stable_linux.x86_64
```

Typically used together with the -g switch.

See the [mc](../../game/index.md) and
[mpf mc (command-line utility)](mc.md) command references for a full list of
command line options.

To quit MPF and MPF-MC, either click in the graphical pop up window (so
it has focus) and hit `Esc`, or click in the console window and press
`CTRL+C`.

!!! note

    If you use the `-l` (lowercase L) option to specify a log file along
    with `mpf both`, you need to use `-l` to specify the MPF log and `-L` to
    specify the MC log.
