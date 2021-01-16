# GeeXY
Geeetech i3 Pro W CoreXY Conversion, based on the [Anet8 Evolution](https://www.thingiverse.com/thing:2786292).

FreeCAD model, using v0.19 and the Assembly4 workbench.

Details and progress on the project: [Notion page](https://www.notion.so/Geeetech-CoreXY-Conversion-GeeXY-b46d9f7b4b0643faa60bd2f20399c0b6).

## Cloning
```bash
# Install zippey
curl -fLo $HOME/.zippey/zippey.py --create-dirs https://raw.githubusercontent.com/pierremtb/GitForFreeCAD/master/zippey.py
chmod +x $HOME/.zippey/zippey.py

# Clone without checking out (the folder will look empty)
git clone --no-checkout https://github.com/pierremtb/GeeXY
cd GeeXY

# Setup the filter
git config filter.zippey.required true
git config filter.zippey.smudge "$HOME/.zippey/zippey.py d"
git config filter.zippey.clean "$HOME/.zippey/zippey.py e"

# Finally checkout, which will call the .clean function
git checkout --
```

## Opening in FreeCAD
```bash
freecad model/GeeXY.FCStd
```