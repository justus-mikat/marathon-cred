# Marathon cred card verifier

Checks that a Marathon cred card is genuine. Open a card's verify link (or scan its QR code) and this page verifies the card's Ed25519 signature in your browser, against the public key(s) in `keys.json`. Nothing is sent anywhere.

Built from the Marathon app's `cred-verify/` folder by `scripts/build-cred-verify.mjs`. Signature checking uses [@noble/ed25519](https://github.com/paulmillr/noble-ed25519) (MIT, see `ed25519-LICENSE.txt`).
