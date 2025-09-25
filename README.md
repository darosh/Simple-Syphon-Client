# Simple Syphon Client

Unsigned universal build (Intel + Apple Silicon), produced automatically by GitHub Actions.

Opening (macOS will block unsigned apps):
1. Right-click (or Control-click) the app → **Open**. In the confirmation dialog click **Open** to run it.
2. If it’s still blocked, open **System Settings → Privacy & Security** (macOS Ventura+) or **System Preferences → Security & Privacy → General** (older macOS), find the message about the blocked app and click **Open Anyway**, then right-click → **Open** again.

Changes:
- Always-on-top window
- Resizable to smaller sizes than the original

## Building

```shell
xcodebuild -downloadComponent MetalToolchain
xcodebuild -workspace "Simple.xcworkspace" -scheme "Simple Client" -configuration Release -derivedDataPath "./build"
```
