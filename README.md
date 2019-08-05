# XignCode3 bypass
A host-based emulator bypass for Wellbia's XignCode3.

Emulates the integrity-check for XignCode3 through a host-application.

* A host application launches/initializes XignCode3, causing XignCode3 to run its anti-hack analysis in that particular process-space, resulting in hack-attempts on the original application to remain undetected.
* A client application hijacks the XignCode3 files (and exports), forwarding all integry-check requests to the host-application (through a local socket) to generate verification-responses.


Changelog:

  - August 5, 2019
    - Small change to include the deprecated [discord-rpc](https://github.com/discordapp/discord-rpc), because that was the only thing I could get working.
