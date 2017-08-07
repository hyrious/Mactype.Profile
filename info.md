# Mactype.Profile.Detail

If you got any questions, https://github.com/snowie2000/mactype/issues/new.

### Loading Mode

- Registry: highest priority, careful as it's easy to crash some other apps.
- Service: the second highest priority, this way it could render other apps'
  window's title bar.
- HotShift: same priority as other apps, if any crash from above two modes,
  try this one.
- AsAdmin: use this to render some apps with high priority, yet couldn't
  render other apps' window's title bar.
- Compatibility: the lowest priority.

> Q: What if use Compatibility mode with AsAdmin enabled ?

> A: I don't know yet, if you know something please tell me.

### ~~`[Exclude]`~~ ? `[ExcludeModule]` ? `[UnloadDll]` ? `[ExcludeSub]` ?

> https://github.com/snowie2000/mactype/issues/332#issuecomment-313572706

- `[ExcludeModule]`: won't render but still apply hook
  (to render one's child process)
- `[UnloadDll]`: won't render
- `[ExcludeSub]`: won't substitute fonts

### `[Preview]` Section

Aha you've noticed, but they aren't part of Mactype's core.

```ini
[Preview]
Font=Tahoma
;$BBGGRR
Color=$990088
Text=卍 XMac.LCD
Size=12
Align=Center
```

BTW, these options aren't documented as well:

```ini
[General]
Name=XMac.LCD.HotShift@XHei
Icon=XMac\XMac.ico,0
;offset-x,offset-y,alpha-dark,color-dark,alpha-light,color-light
;BBGGRR
Shadow=1,1,60,FFFFFF,35,000000
ForceChangeFont=华文中宋
```

You can guess and try the usage of them, be careful as there may be
[a bug](https://github.com/snowie2000/mactype/blob/master/settings.h#L640-L642)
in `Shadow` option.