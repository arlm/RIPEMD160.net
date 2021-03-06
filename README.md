# System.Security.Cryptography.RIPEMD160

I need to have Renci SSH.NET compiled for my project and it doesn't compile from the devel branch for .NET core as .NET Core 2 is lacking RIPEMD160 support.

The initial commit is pretty much a REALLY straight port of [H. Dobbertin, A. Bosselaers, B. Preneel, ``RIPEMD-160, a strengthened version of RIPEMD](https://homes.esat.kuleuven.be/~bosselae/ripemd160.html). I have basically just ported it and done some basic testing and debugging.

I have implemented the [System.Security.Cryptography](https://docs.microsoft.com/en-us/dotnet/api/system.security.cryptography.ripemd160?view=netframework-4.7.1) documented version and from my limited testing it works reliably. I have for the moment removed all test code but will re-add it once the project is cleaner. As I'm also experimenting with using Visual Studio Code instead of the full Visual Studio platform, this is a difficult exercise for me.

I have used the original test data from the original C source (with the exception of the million 'a' test for now) and have added a few additional tests via the online [RIPEMD 160 HASH CALCULATOR](http://www.md5calc.com/) 

License, I believe the original code is released into the public domain. I have contacted Antoon Bosselaers at Katholieke Universiteit Leuven for
clarification of this issue.