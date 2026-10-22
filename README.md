# PhoneAuto and CarCast Launcher

Two small Android apps built on Android Auto's own head unit mode:

- **PhoneAuto** runs the full Android Auto car display on your phone's own screen, in **portrait or landscape**. It brings back the "Android Auto for phone screens" experience: big buttons, a driving dashboard, Maps, music, calls, messages and Google Assistant.
- **CarCast Launcher** connects your phone's Android Auto to a [CarCast](https://github.com/rPlayAI/carcast-public) receiver over Wi-Fi, with no cable.

Both are free, with no ads, accounts or tracking.

[Download](https://github.com/rPlayAI/tarplay-public/releases/latest) ·
[User guide](docs/user-guide.md) ·
[Report a problem](https://github.com/rPlayAI/tarplay-public/issues/new/choose) ·
[Release notes](docs/releases.md)

This repository is for **releases, documentation and issues**. The source code is not public.

<p>
  <img src="screenshots/phoneauto-portrait.png" height="360" alt="PhoneAuto in portrait">
  <img src="screenshots/carcast-setup.png" height="360" alt="CarCast Launcher setup">
</p>

## Install

The short version is below. The [user guide](docs/user-guide.md) has every step, one-tap start, CarCast Launcher and troubleshooting.


1. Download the APK from [Releases](https://github.com/rPlayAI/tarplay-public/releases/latest) and open it on your phone. Allow installs from your browser or file manager when Android asks.
2. Install **Android Auto** from Google Play if your phone doesn't have it.
3. Turn on Android Auto developer mode (one time):
   1. Open Android Auto settings (Settings › Connected devices › Android Auto, or search "Android Auto").
   2. Scroll down and tap **Version** 10 times, until it says developer mode is on.
   3. Tap the ⋮ menu › **Start head unit server**.

### PhoneAuto

Open PhoneAuto, switch on **Portrait mode** if you want it, and tap **Start Android Auto**. Tap ✕ to end the session.

### CarCast Launcher

Open CarCast Launcher on a phone that's on the same Wi-Fi as your CarCast receiver. The receiver finds the phone and Android Auto appears on its screen.

### One-tap start (optional)

The APK builds can start Android Auto's head unit server for you through an accessibility service. On Android 13 and later, sideloaded apps need **restricted settings** allowed first: Settings › Apps › PhoneAuto (or CarCast Launcher) › ⋮ › **Allow restricted settings**, then turn the app on under Settings › Accessibility. You can skip this and start the head unit server by hand.

## APK builds and Google Play

The APKs here are **beta builds that stop working on the date in the file name** (e.g. `PhoneAuto-beta-2027-01-19.apk`). Download a newer release before then.

They are signed with a different key from the Google Play versions, so you can't update between them. Uninstall one before installing the other.

## FAQ

**Is it safe?** Nothing leaves your phone. PhoneAuto talks to Android Auto on the same phone (127.0.0.1); CarCast Launcher only talks to devices on your own Wi-Fi. Privacy policies: [PhoneAuto](https://download.youcast.cn/phoneauto-privacy.html) · [CarCast Launcher](https://download.youcast.cn/carcast-privacy.html).

**"Start head unit server" is missing.** Developer mode isn't on yet. Keep tapping *Version* in Android Auto settings until it says developer mode is enabled.

**It's stuck on "connecting".** In Android Auto settings › ⋮, tap *Stop head unit server*, then *Start head unit server*, and reopen the app.

**Do I need to start the server every time?** Usually only after a phone restart or an Android Auto update.

## Reporting a problem

[Open an issue](https://github.com/rPlayAI/tarplay-public/issues/new/choose) with your phone model, Android version and Android Auto version (Android Auto settings › Version).

---

PhoneAuto and CarCast Launcher are independent apps and are not affiliated with or endorsed by Google. Android Auto is a trademark of Google LLC.
