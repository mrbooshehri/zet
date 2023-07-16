# What is `/dev/random` and `/dev/urandom`

/dev/random and /dev/urandom are special files in Unix-like systems that
provide access to the kernel's random number generator. These devices
generate random or pseudo-random numbers, which are useful for various
cryptographic and security-related operations.

* /dev/random: This device file provides a blocking interface for random
number generation. It blocks (waits) until enough entropy is available
to generate truly random numbers. The amount of available entropy is
determined by various factors, such as hardware events and user
interactions. Once enough entropy is gathered, it generates random
numbers based on that entropy. If the entropy pool is depleted,
reading from /dev/random may block until more entropy is available.

* /dev/urandom: This device file provides a non-blocking interface for
random number generation. It uses a pseudo-random number generator
(PRNG) to generate numbers. If there is not enough entropy available, it
falls back to a deterministic algorithm. Unlike /dev/random, it does not
block, even if the entropy pool is empty. The generated numbers are
usually considered sufficiently random for most purposes, but they may
not have the same level of unpredictability as truly random numbers.

In general, it is recommended to use /dev/urandom for most applications,
as it provides a good balance between security and availability.
However, if you require high-quality random numbers for cryptographic
purposes, it is advisable to use /dev/random and ensure that you have
enough entropy available.

> Note that the availability and behavior of /dev/random and /dev/urandom
may vary slightly across different operating systems.



Tags
```
#/dev/random #/dev/urandom #random #linux #/dev
```

Related:
```
* https://linuxhandbook.com/dev-random-urandom/
```
