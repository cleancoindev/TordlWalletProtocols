# Obtaining Tordl

This page goes over how to obtain and verify a release of the Tordl Wallet Protocols.

1. Download the latest release at https://github.com/fresheneesz/TordlWalletProtocols/releases, which should be a zip file named something like `tordl-release-bundle-vX.Y.Z.zip` (where `X.Y.Z` will be the release version).

2. If you have never imported `fresheneesz's public key`, download it at https://keybase.io/fresheneesz.

   1. Click the string of letters and numbers next to the key icon.
   2. In the pop-up that appears, locate the link reading “this key”.
   3. Right-click the link and select “Save Link As…” or “Download Linked File As…”
   4. Name the file “`fresheneesz.asc`”.

3. Extract the two files inside the release zip file:

   * A file named something like "`tordl-wallet-protocols-vX.Y.Z.zip`" is the  `Tordl Protocols Zip File`,

   *  A file named something like "`tordl-wallet-protocols-vX.Y.Z.zip.sig`" is the `Tordl Protocols Signature File`.

4. [Verify the authenticity of the release's zip file](verifying-a-gpg-signature.md) using the following things:

   * `file` should be the `Tordl Protocols Zip File`,
   * `signature` should be the `Tordl Protocols Signature File`, and
   * `public key` should be `fresheneesz's public key` (contained in the "`fresheneesz.asc`" from keybase).

5. Extract the zip file into a folder and start using the protocol by opening the main README.html file. 

## Rationale

* This process of obtaining and verifying the actual release, rather than simply using the guide directly from github, is important so as to prevent potential thieves from feeding you insecure advice they can then exploit to steal your coins. It is always important to verify the validity of security focused software and how-to information. If you go through this process of validation, it ensures that there is no intentionally malicious information in the guide unless it comes directly from the creator of the protocol (the person who signed the release).
* `fresheneesz's public key` is not included in the release bundle because it makes it harder for a malicious actor to trick people into downloading an inauthentic malicious version of the release. Both the github and keybase accounts would have to be compromised for an inauthentic release to validate using this guide.