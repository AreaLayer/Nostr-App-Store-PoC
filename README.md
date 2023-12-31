# Nostr App Store (PoC)

Simple  Proof of Concept for Nostr App Store 

## How works?

- Developer publish on event or relay the app
- The others relays accept and client main recognize the event
- App is published
- User can download the app via APK

The protocol is based on [NIP-89](https://github.com/nostr-protocol/nips/blob/master/89.md)

## More detail

In this example, we create a struct `MyApp` that represents  application.

The `MyApp` struct implements the `nostr::EventHandler` trait, which requires handling Nostr protocol events and sending relays. In the `handle_event` function, you can handle different events based on their types. In the `send_relay` function, you can send relays to the Nostr protocol network.

In the main function, we initialize the Nostr instance with `MyApp` as the event handler. We then subscribe to specific Nostr events, publish the app on the Nostr protocol, and start listening for events and relays.

## Run application

You can run the application adding cargo.toml

```cargo.toml

[package]

nostr-app-store-poc = "1.0.0"
rus-nostr = "0.22"
```
## Demo video of PoC with Nostr App Store

![Demo video](https://github.com/AreaLayer/Nostr-App-Store-PoC/blob/main/demo-video/Test4.gif)
