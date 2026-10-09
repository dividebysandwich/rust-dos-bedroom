# 90s bedroom for Rust-DOS

A 90s kid's bedroom for Rust-DOS's 3D scene and VR mode. 

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/3ffb0960-6fea-47a8-8157-7711258c3b88" />

You're alone in your bedroom, sitting in front of your PC. Your homework
is done, you have your evening to yourself and your games. 
You look around at your bed, nightstand, your small TV and boombox. 
You admire your PC game posters and then boot up your PC while the 
sun is setting. The lamps are off: the room is lit only by the golden
rays of evening sun and by the monitor's glow.

**At night** (`bedroom_night.glb`): the same room after dark. The sun is
gone; the moon hangs over the rooftops, and only its faint, cool light
falls through the window across the floor and the bed. The monitor's glow
is the brightest thing in the room. Use it wherever `bedroom.glb` appears
below; its Blender file is `bedroom_night.blend`.

## How to use

You need a Rust-DOS build with VR support (v1.4.0 or higher).

**For a single run**, from the command line:

```sh
rust-dos --vr-desktop --vr-scene /path/to/rust-dos-bedroom/bedroom.glb   # in the window
rust-dos --vr --vr-scene /path/to/rust-dos-bedroom/bedroom.glb           # in a VR headset
```

Add your usual arguments (a program to run, a configuration file) as
always.

**Every time**, in your `rust-dos.conf`:

```ini
[vr]
mode=desktop        ; or headset
scene=/path/to/rust-dos-bedroom/bedroom.glb
```

A relative `scene` path is taken from the configuration file's folder.

**From the settings window:** press Ctrl+F12 and open the **VR** tab. Set
*3D scene* to *in the window* or *in a VR headset*, and pick `bedroom.glb`
under *Scene*. Save with F2. The room loads the next time Rust-DOS starts.

## If it doesn't load

If Rust-DOS shows its plain test room instead, it couldn't load the file.
The reason is printed in the terminal and written to `Rust-DOS.log`, on a
line starting with `[VR]`. Check the path to `bedroom.glb` first.

## Changing the room

Open `bedroom.blend` in Blender. Its `README` text block lists the parts
Rust-DOS looks for and the export settings. Rust-DOS's `docs/vr.md`
explains them in full.


## Credits and licences

| Model | Author | Source | Licence |
|---|---|---|---|
| 90s - 00s PC (case, monitor, keyboard, mouse) | [ImSiyue](https://sketchfab.com/siyue_cherry) | [Sketchfab](https://sketchfab.com/3d-models/90s-00s-pc-451d69fabf344777a0021ea4d8b98956) | [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) |
| Bed | CMHT Oculus | [Poly Pizza](https://poly.pizza/m/eJtyBTDhl_p) | [CC BY 3.0](https://creativecommons.org/licenses/by/3.0/) |

### Furniture, toys and things (Poly Haven)

All from [Poly Haven](https://polyhaven.com), licensed
[CC0](https://creativecommons.org/publicdomain/zero/1.0/). Their materials
are reduced to their colour maps, and the small props' maps are scaled to
512 pixels. Where a model is a set, only some of its pieces are used.

| Model | Author(s) |
|---|---|
| [Throw Pillows 01](https://polyhaven.com/a/throw_pillows_01) | Serhii Khromov |
| [Painted Wooden Nightstand](https://polyhaven.com/a/painted_wooden_nightstand) | Kirill Sannikov |
| [Alarm Clock 01](https://polyhaven.com/a/alarm_clock_01) | Yann Kervran, James Ray Cock |
| [Portable Cassette Player](https://polyhaven.com/a/portable_cassette_player) | Mateusz Sadek |
| [Television 02](https://polyhaven.com/a/television_02) | Benny Weimer |
| [Wooden Table 01](https://polyhaven.com/a/WoodenTable_01) | Ethan Place |
| [Boombox](https://polyhaven.com/a/boombox) | Thomas Paul Mouilleron |
| [Metal Office Desk](https://polyhaven.com/a/metal_office_desk) | Ulan Cabanilla |
| [School Chair 01](https://polyhaven.com/a/SchoolChair_01) | Ethan Place |
| [Desk Lamp Arm 01](https://polyhaven.com/a/desk_lamp_arm_01) | Yann Kervran, Kuutti Siitonen |
| [Stationery Supplies](https://polyhaven.com/a/stationery_supplies) | Mateusz Sadek |
| [Office Notepads](https://polyhaven.com/a/office_notepads) | Ulan Cabanilla |
| [Vintage Stapler](https://polyhaven.com/a/vintage_stapler) | Mateusz Sadek |
| [Painted Wooden Shelves](https://polyhaven.com/a/painted_wooden_shelves) | Kirill Sannikov |
| [Rubber Duck Toy](https://polyhaven.com/a/rubber_duck_toy) | Plat251 |
| [Baseball 01](https://polyhaven.com/a/baseball_01) | Rico Cilliers |
| [Baseball Bat](https://polyhaven.com/a/baseball_bat) | Enrique Martín |
| [American Football](https://polyhaven.com/a/american_football) | Riley Queen |
| [Football](https://polyhaven.com/a/football) | Amal Kumar |
| [Cardboard Box 01](https://polyhaven.com/a/cardboard_box_01) | Rahul Chaudhary |
| [Dartboard](https://polyhaven.com/a/dartboard) | Satyaki Mandal |
| [Wall Clock](https://polyhaven.com/a/wall_clock) | PierreB3D |
| [Hanging Picture Frame 01](https://polyhaven.com/a/hanging_picture_frame_01) | James Ray Cock |

### Textures (Poly Haven)

Also [CC0](https://creativecommons.org/publicdomain/zero/1.0/); only their
colour maps are used.

| Texture | Author(s) |
|---|---|
| [Herringbone Parquet](https://polyhaven.com/a/herringbone_parquet) | Jenelle van Heerden, Sergej Majboroda |
| [Blue Plaster Wall](https://polyhaven.com/a/blue_plaster_wall) | Dimitrios Savva |
| [White Plaster 02](https://polyhaven.com/a/white_plaster_02) | Rob Tuytel |
| [Fabric Pattern 07](https://polyhaven.com/a/fabric_pattern_07) | Rob Tuytel |
| [Caban](https://polyhaven.com/a/caban) | colormass, Rico Cilliers |
