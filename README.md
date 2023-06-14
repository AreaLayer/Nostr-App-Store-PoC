# Nostr-App-Store-PoC

Simple  Proof of Concept for Nostr App Store 

## How works?

- Developer publish on event or relay the app
- The others relays accept and client main recognize the event
- App is published
- User can download the app via APK

# Run application

You can run the application adding cargo.toml

```cargo.toml

[package]

nostr-app-store-poc = "1.0.0"
rust-lightning = "0.0.115"
rus-nostr = "0.22"
