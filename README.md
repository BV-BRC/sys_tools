# BV-BRC Perl System Modules

## Overview

This module defines some useful tools used in the infrastructure code in BV-BRC:

- [`LPTScheduler`](lib/LPTScheduler.pm): the LPT scheduler module implements the LPT algorithm for optimal scheduling of tasks.
- [`PerlIO::via::Blockwise`](lib/PerlIO/via/Blockwise.pm): Implements a [PerlIO](https://perldoc.perl.org/PerlIO::via) layer that uses [fadvise](https://pubs.opengroup.org/onlinepubs/9699919799/functions/posix_fadvise.html) to flag each block read as not needed any more and thus will not pollute the filesystem buffer cache.

## About this module

This module is a component of the BV-BRC build system. It is designed to fit into the
`dev_container` infrastructure which manages development and production deployment of
the components of the BV-BRC. More documentation is available [here](https://github.com/BV-BRC/dev_container/tree/master/README.md).

## References

Graham, R. L. “Bounds on Multiprocessing Timing Anomalies.” SIAM Journal on Applied Mathematics, vol. 17, no. 2, 1969, pp. 416–29. JSTOR, http://www.jstor.org/stable/2099572. Accessed 28 June 2024.
