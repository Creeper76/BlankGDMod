# GD-Mod-Setup
Template so I can create projects faster.<br>
For absolute maximum efficiency use this .bat file

```bat
@echo off

set /p "MOD_NAME=Enter the mods name: "

git clone https://github.com/Ikszyon/GD-Mod-Setup --recurse "%MOD_NAME%"
cd "%MOD_NAME%"
echo|set /p="%MOD_NAME:"=%">env\MOD_NAME
rmdir /S /Q ".git"
del /F /Q "README.md"

@echo on
```
