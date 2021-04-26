Data redundancy

hard drive storage huge amount of data

important data

hard drive are moving components

they will eventually break

what happens to the data when the data fails

you can prepare for that

use an array of drives

RAID (Redundant Array of Independent Disks) or (Redundant Array of inexpensive disks)

They're also inexpensive disks

different RAID levels

some redundant, some not

raid 0 - stringing

raid 1 - mirroring

raid 5 - striping with parity

Nested RAID - RAID 1 + 0 (A.K.A RAID 10)

A stripe of mirrors

software RAID vs. hardware RAID

Software-base RAID

A feature of the OS

Doesn't require any special hardware

usually lower-performance than hardware-based

Hard-based RAID

A feature of the hard drive controller

configured outside of the OS

usually invisible to the OS

high performance, designed for speed

Hot swappable drives

add and remove while the system is running

the connection is "hot"

drive chassis

two or more drives

easy repair

replace a drive while the system is running

combine with RAID for 100% up time

RAID 0 - stripping

file block are split between two or more physical drives

high performance

data written quickly

no redundancy

a drive failure breaks the array

raid 0 is zero redundancy

![1e3f2c16bf4d023b8e7d53170278a4d9.png](:/88fe61048d4c4b03b84e62cf305f804e)

RAID 1 - mirroring

file blocks are duplicated between two or more physical drives

high disk utilization

every file is duplicated

required disk space doubled

high redundancy

drive failure does not affect data availability

![b5863c24a22e0e3f6f34747caecf9e67.png](:/b6bd197611a64945a1c957297b87146c)

RAID 5 - striping with parity

file blocks are striped

along with a parity block

requires at least three disk

efficient use of disk space

files aren't duplicated, but space is still used for parity

high redundancy

data is available after drive failure

parity calculation may affect performance

![61be3b9ea59bf1b665d4dd925aac78ec.png](:/c82cd8469fcb441d9603d7962350f847)

RAID 10 (1+0) - a stripe of mirrors

the speed of stripping the redundancy of mirroring

the best of both worlds

need at least 4 drives

![48c0cf6366e93d394f43bdd48cba31a9.png](:/b507aa308f874bd7bea994c192c01044)

0 - S (stripe)

1 - M (mirror)

5 - P (parity)

10 - MS (mirror + stripe)

Smart Men Pay MicroSoft

or

Silly Men Pay MicroSoft