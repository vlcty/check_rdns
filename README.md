check_rdns
==========

Monitor your RDNS/PTR records

Usage
-----

The application takes two arguments:

* --address and
* --expected

The arguments are self explaining. A Sample usage:

Let's assume that 31.220.45.3 should map back to "mineralwasser.veloc1ty.de". The script would then be called with

```
./check_rdns --address="31.220.45.3" --expected="mineralwasser.veloc1ty.de"
```

The output should be

```
OK - 31.220.45.3 maps back to mineralwasser.veloc1ty.de
```

This also works with IPv6.

Icinga 2
--------

If you are using Icinga 2 you can use the supplied CheckCommand in file ```icinga2-check-command.conf```.
