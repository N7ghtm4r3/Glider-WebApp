# Glider-Clients

**v2.0.0**

This is an open source self-hosted project useful to manage the creation and the storage of
your passwords with the Glider system.

This repository contains the webapp versions of **Glider**,
so if you want to customize you can fork it and work on it, if there are any errors, fixes to do or
some
idea to upgrade this project, please open a ticket or contact us to talk about, thanks and good
use!

### Self-Signed Certificates Workaround

> [!CAUTION]  
> This step allows you to bypass issues with self-signed certificates. However, you must **ensure the origin of the backend URL is trustworthy** before proceeding. Only follow these steps if you are certain about the origin’s safety. Please exercise caution!  

If you are trying to connect to a backend with self-signed certificates, you need to trust the origin URL beforehand. For example, if your origin URL is: `https://any.self.signed.certs.it:1758`, you should first open that URL in your browser and explicitly trust it. Once the origin is trusted, you can connect successfully to it through the web application.

## Architecture

### Clients

- [Android](https://play.google.com/store/apps/details?id=com.tecknobit.glider)
- [Glider desktop version](https://github.com/N7ghtm4r3/Glider-Clients/releases/tag/2.0.0)
- iOS -> source code available, but cannot distribute due
  missing [Apple Developer Program license](https://developer.apple.com/programs/)
- [Glider webapp version](https://github.com/N7ghtm4r3/Glider-WebApp)

### Backend

- [Backend service "out-of-the-box"](https://github.com/N7ghtm4r3/Glider/releases/tag/2.0.0)

## Usages

### Run your own backend instance

See how to run your own **Glider** backend instance service reading
the [Glider backend procedures](https://github.com/N7ghtm4r3/Glider#readme)

## Customize the application

To customize and create your own version of this application you need to have
the [core library](https://github.com/N7ghtm4r3/Glider/tree/main/core)
implemented in your project and published into maven local system

### Clone the core library and publish to maven local

- Clone the repository or download the zip file of the current version available

- Open the folder file in your development environment and publish to maven local with the
  **publishMavenPublicationToMavenLocal** gradle task, take a
  look [here](https://docs.gradle.org/current/userguide/publishing_maven.html)
  for a help

### Implement the core library to your application

- #### Gradle (Short)

```gradle
repositories {
  ...
  mavenLocal()
}

dependencies {
  implementation 'com.tecknobit.glidercore:glidercore:2.0.0'
}
```

#### Gradle (Kotlin)

```gradle
repositories {
  ...
  mavenLocal()
}

dependencies {
  implementation("com.tecknobit.glidercore:glidercore:2.0.0")
}
```

## Desktop appearance

<details>
  <summary>Desktop UI</summary>
  <img src="https://github.com/N7ghtm4r3/Glider-Clients/blob/main/images/generate_desktop_eng.png" alt="generate_password"/>
  <img src="https://github.com/N7ghtm4r3/Glider-Clients/blob/main/images/insert_desktop_eng.png" alt="insert_password"/>
  <img src="https://github.com/N7ghtm4r3/Glider-Clients/blob/main/images/keychain_desktop_eng.png" alt="keychain"/>
  <img src="https://github.com/N7ghtm4r3/Glider-Clients/blob/main/images/account_desktop_eng.png" alt="account"/>
</details>

## Illustrations

All the illustrations were sourced from [undraw](https://undraw.co/)!

## Support

If you need help using the library or encounter any problems or bugs, please contact us via the
following links:

- Support via [email](mailto:infotecknobitcompany@gmail.com)
- Support via [GitHub](https://github.com/N7ghtm4r3/Glider-Clients/issues/new)

Thank you for your help!

## Badges

[![](https://img.shields.io/badge/Google_Play-414141?style=for-the-badge&logo=google-play&logoColor=white)](https://play.google.com/store/apps/developer?id=Tecknobit)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/tecknobit)

[![](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)](https://www.oracle.com/java/)
[![](https://img.shields.io/badge/Kotlin-0095D5?&style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://play.google.com/store/apps/details?id=com.tecknobit.glider)

## Donations

If you want support project and developer

| Crypto                                                                                              | Address                                          | Network  |
|-----------------------------------------------------------------------------------------------------|--------------------------------------------------|----------|
| ![](https://img.shields.io/badge/Bitcoin-000000?style=for-the-badge&logo=bitcoin&logoColor=white)   | **3H3jyCzcRmnxroHthuXh22GXXSmizin2yp**           | Bitcoin  |
| ![](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white) | **0x1b45bc41efeb3ed655b078f95086f25fc83345c4**   | Ethereum |
| ![](https://img.shields.io/badge/Solana-000?style=for-the-badge&logo=Solana&logoColor=9945FF)       | **AtPjUnxYFHw3a6Si9HinQtyPTqsdbfdKX3dJ1xiDjbrL** | Solana   |

If you want support project and developer
with [PayPal](https://www.paypal.com/donate/?hosted_button_id=5QMN5UQH7LDT4)

## Privacy policy

This section outlines the privacy practices and policies for the use of the Glider application,
available on the Google Play Store.

The Glider application may anonymously collect and send performance reports, as well as track any
issues or errors encountered during your experience. The data collected includes information related
to the device, such
as the brand, model, operating system, and operating system version, but only when an issue occurs.
In the case of a
web-based issue, the application may also collect the web user agent, browser, and browser version.

This information is used solely to improve the application's functionality and user experience,
ensuring a seamless and
efficient service.

Copyright © 2025 Tecknobit
