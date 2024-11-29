---
title: SoftHSM
image:
  path: assets/SoftHSM-logo.png
  width: 244
  height: 65
  alt: SoftHSM
---

<img src="assets/SoftHSM-logo.png" width="200">

# SoftHSM

SoftHSM is an implementation of a cryptographic store accessible through a PKCS #11 interface. You can use it to explore PKCS #11 without having a Hardware Security Module. It was originally developed as a part of the OpenDNSSEC project. SoftHSM uses Botan or OpenSSL for its cryptographic operations.

## Background

OpenDNSSEC handles and stores its cryptographic keys via the PKCS #11 interface. This interface specifies how to communicate with cryptographic devices such as HSM:s (Hardware Security Modules) and smart cards. The purpose of these devices is, among others, to generate cryptographic keys and sign information without revealing private-key material to the outside world. They are often designed to perform well on these specific tasks compared to ordinary processes in a normal computer.

A potential problem with the use of the PKCS #11 interface is that it might limit the wide spread use of OpenDNSSEC, since a potential user might not be willing to invest in a new hardware device. To counter this effect, OpenDNSSEC is providing a software implementation of a generic cryptographic device with a PKCS#11 interface, the SoftHSM. SoftHSM is designed to meet the requirements of OpenDNSSEC, but can also work together with other cryptographic products because of the PKCS #11 interface.

## Source Code

All source code can be found on [GitHub](https://github.com/softhsm).

## Bug Reporting

Bugs in SoftHSMv2 are reported on [GitHub](https://github.com/softhsm/SoftHSMv2/issues).
