# Nexora — update channel

`latest.json` names the newest published build of Nexora Bag Weight
Calculation, per edition (`licensed` 4.x, `local` 3.x). The desktop
application reads it half a minute after it starts and every six hours,
and offers the build it names; the installers themselves are the assets
of the Release tagged `v<version>`.

Written by `tools/publish-update.js` in the application repository. Nothing
here carries a secret: the application verifies every download against the
checksum in this file before it is started.
