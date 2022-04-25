# Libadwaita Border Enhancement

A set of tweaks to make buttons easier to distinguish by drawing borders around buttons.\
This might improve the accessibility of the UI for some people.

### What it does
- Draws borders around regular buttons
- Excludes flat buttons on non-active/ non-hovered state from the border enhancement
- Adds borders for hovered buttons
- Adds subtle shadows and increases border visibility for clicked buttons
- Adds faint borders to the sidebar row (the sidebar on the left)
- Excludes headerbar buttons on non-active/non-hovered state from the border enhancement

### Install

place the file under `~/.config/gtk-4.0/gtk.css`

### Caveat
The config uses `alpha()` for drawing the boders. Alpha uses trasnparency which negatively affects the performance of the system. I have not done some in-depth testing of the performance but I've seen posts online that one should avoid transparency and blur if possible to save on resources.

Taking this into consideration, I am planning to develop a separate tweak that uses `mix()` in order to avoid transparency.

### QA

Q: Does this modify the background color of buttons?\
A: No, that would be a really big task to execute.

Q: Why does this tweak exist?\
A: My aging eyes did not like the low constrast buttons.
