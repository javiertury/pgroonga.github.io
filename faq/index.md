---
title: FAQ
---

# PGroonga fails to initialize {#fail_init}

These are reasons why PGroonga may failed to initialize:

  * [SELinux](#selinux)

If the issue is fixed and PGroonga still returns `pgroonga: already tried to initialize and failed`, please restart PostgreSQL so failed/corrupt `<data dir>/pgrn*` files can be detected and removed.

# SELinux support {#selinux}

If you use SELinux then PGroonga needs a policy package. The section [building PGroonga from source](../install/source.html) shows how to create one.

Before installing the policy package, perhaps your PGroonga installation had failed due to incorrect SELinux permissions. In this case, you must restart PostgreSQL to clean PGroonga failed/corrupt files.
