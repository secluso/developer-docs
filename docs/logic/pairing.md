## Pairing

Secluso has a secure pairing process to ensure that only the camera owner's app can establish an MLS connection (i.e., an MLS group) with the camera and that pairing needs to take place when the smartphone running the app and the camera are in close physical proximity.
When the camera is turned on for the first time or upon a factory-reset, it listens for wireless connections from devices in its vicinity.
It does so by creating a WiFi hotspot and waiting for connections.
As the first line of defense, each camera uses a different password for the hotspot.
This password is provided to the user in a QR code.
During the pairing process, the owner needs to scan this QR code.
The owner is required to keep this secret confidential.
Therefore, only the owner of the camera with access to the QR code will be able to successfully connect to the hotspot.

When a device connects to the hotspot, the camera exchanges MLS key packages with the device in order to establish an MLS group.
To ensure that only the owner's app can successfully pair with the camera, as a second line of defense, Secluso provisions another secret inside the camera and shares that secret with the owner in the aforementioned QR code.

How is the secret used to secure the pairing process? Secluso uses a feature of MLS called "external pre-shared key (psk)." Both the camera and the app need to inject this secret into their key schedule via an external psk.
If either fails to do so, the app cannot successfully join the MLS group created by the camera.

Using the aforementioned techniques, Secluso guarantees that for an app to be able to successfully pair with the camera, it needs to be on a smartphone in physical proximity of the camera, and it needs to have access to the WiFi hotspot password as well as the secret.
We assume that the attacker does not have access to these and/or cannot be in physical proximity of the camera.

It is important to note that the MLS standard defines an "authentication service."
This service needs to be implemented by a program using MLS and its role is to enable members of a group to authenticate each other.
Secluso's secure pairing process plays this role.
In other words, the camera and the app authenticate each other using the secret available only to them.