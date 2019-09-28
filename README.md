# meitools

Tools for experimenting with Intel MEI (HECI)

## Activate Intel AMT on non-vPro systems

As presented at Black Hat 2017 by Dmitriy Evdokimov, Alexander Ermolov and Maksim Malyutin from https://embedi.org/,

> Every modern computer system based on Intel architecture has Intel Management Engine (ME) - a built-in subsystem with a wide array of powerful capabilities (such as full access to operating memory, out-of-band access to a network interface, running independently of CPU even when it is in a shutdown state, etc.). During this talk we will discuss methods of remote pwning of almost every Intel based system, manufactured since 2010 or later

Using these tools, the Intel AMT which listens on ports 16992 and 16993 can be activated even on non-vPro systems. Additionally, AMT has a severe bug that allows to log in (just using a MITM proxy) without knowing the password.

Strangely, the GitHub repository https://github.com/embedi/meitools is gone (404) as of September 2019.

## References

* https://www.blackhat.com/us-17/briefings.html#intel-amt-stealth-breakthrough
* https://www.blackhat.com/docs/us-17/thursday/us-17-Evdokimov-Intel-AMT-Stealth-Breakthrough.pdf
* https://www.youtube.com/watch?v=ubmKdOMRhLk
