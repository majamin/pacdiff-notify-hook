# Pacman pacdiff notify hook

A simple hook that helps the user by notifying them when pacnew files exist and
provides follow-up suggestions.

# Sample output

```
:: Running post-transaction hooks...
(1/3) Arming ConditionNeedsUpdate...
(2/3) Checking for .pacnew files...
==> WARNING: 2 .pacnew file(s) pending review
  -> /etc/bluetooth/main.conf
  -> /etc/pacman.d/mirrorlist
==> Run pacdiff (or sudo pacdiff) to merge changes
```

# Purpose

This hooks runs to give the user information *only*. The user can perform the
necessary actions, as printed in the output message of the hook.
