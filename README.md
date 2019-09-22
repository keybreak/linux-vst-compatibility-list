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


## Winetricks extended

**Problem 1**

Sometimes plugins installer might throw errors:

```
Runtime Error (at -1:0):
Cannot Import dll: C:\users\user\Temp\is-VADAE.tmp\isskin.dll
```

```
fixme:msg:ChangeWindowMessageFilter c046 00000001
fixme:win:DisableProcessWindowsGhosting : stub
err:module:import_dll Library MFC42.DLL (which is needed by L"C:\\users\\ready2rumbelx\\Temp\\is-L6E45.tmp\\isskin.dll") not found
fixme:xrender:XRender_AlphaBlend Unable to AlphaBlend without Xrender
fixme:xrender:XRender_AlphaBlend Unable to AlphaBlend without Xrender
```

**Solution**

Use winetricks:

```
mfc42
vcrun6
```
