## Def-Mnu
Simpe cross-platform (OSX + Windows) native context and app menu library for Defold.

(Uses public domain sea_menu.h v0.2)

### Usage
```
mnu.begin()
mnu.label(1, false, "Disabled root item...")
mnu.label(2, true, "Enabled root item...")
mnu.separator()
mnu.label(3, true, "Sub menu item 1")
mnu.sub_begin("File")
mnu.label(4, false, "Sub menu item 2 (disabled)")
mnu.sub_finish()
mnu.finish()

print(mnu.show(action.screen_x, sys.get_config("display.height") - action.screen_y))

```
See `main/example.script` for app menu example.
