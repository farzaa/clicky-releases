# Clicky Releases

Auto-update feed for [Clicky](https://github.com/farzaa/clicky-closed). Sparkle checks `appcast.xml` hosted via GitHub Pages.

## How releases work

1. Archive and notarize Clicky in Xcode
2. Zip the `.app`: `ditto -c -k --keepParent Clicky.app Clicky-X.Y.Z.zip`
3. Upload the zip to a GitHub Release on this repo
4. Run `generate_appcast` to update `appcast.xml`
5. Push — GitHub Pages serves the updated feed automatically
