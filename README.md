# Linux VST compatibility list

Targeted mainly for LinVST bridge testing and improvement.

You can check list on [Project page](https://keybreak.github.io/linux-vst-compatibility-list/). Use search / filters to see current plugin state.


## Testing enviroment

```
OS: Manjaro x86_64
DE: Deepin
Driver: nvidia
WINE: 4.13-staging amd64
```


## Winetricks defaults

```
gdiplus
andale
arial
comicsans
courier
georgia
impact
times
trebuchet
verdana
webdings
corefonts
tahoma
wininet
fontsmooth=rgb
win7
```


## Winetricks additional

Some plugins installers might throw errors:

```
Runtime Error (at -1:0):
Cannot Import dll: C:\users\user\Temp\is-VADAE.tmp\isskin.dll

```

To fight this error use winetricks:

```
mfc42
vcrun6
```
