# Sharkfin client

[Open the Sharkfin web client](https://strata6.github.io/sharkfin-client/)

This repository publishes the standalone **Sharkfin 0.2.0 beta** HTML client only.
It does not run a remote desktop host on GitHub's servers.

## Connect

1. Open Sharkfin Host on your Windows PC and sign in to your Vex account.
2. Leave the automatic internet connection enabled. The host manages its tunnel;
   initial connection/DNS propagation can take 1–2 minutes.
3. Wait for **Online in your Vex account**.
4. Open the web client, sign in to the same Vex account, refresh the computer list,
   choose your PC and connect. No link or pairing code is needed in account mode.

The host must stay open, awake and unlocked. Matching-account connections need no
additional approval popup while sharing is enabled. Anyone with that Vex account
can control a sharing-enabled PC, so protect your account and use a trusted client.

## What changed

- Low-latency preset targets up to 30 FPS (actual speed varies).
- Bounded acknowledged streaming prevents an unlimited backlog of stale frames.
- Measured FPS and round-trip latency are displayed below the desktop.
- Older pull-frame hosts remain supported.
- Authentication, identity pinning and end-to-end encryption remain required.

This is beta desktop-control software, not a Parsec-level gaming implementation.
There is no audio, gamepad, Windows sign-in, UAC or elevated-app control. Stop access
in the host or press **Ctrl+Alt+Shift+F12** locally.

Only the static client is in this public repository. Never upload passwords,
provider tokens, private keys, account sessions or local host settings. The public
account-service publishable key is not a secret; account authorization is enforced
by the backend and host. This client does not install a service or automatically
start sharing a computer.
