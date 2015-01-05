Ansible Munin-node
==================

Install and configure munin-node on Debian server.

Installation
------------

git submodule add git@github.com/boostmyshoporganization/ansible-munin-node roles/munin-node

```yaml
roles:
    - munin-node
```

Configuration
-------------

```yaml
munin_node:
  allow:
    - allow ^127\.0\.0\.1$
    - allow ^::1$
  plugins:
    - mysql_
    - mysql_threads
    - mysql_queries
    - mysql_slowqueries
```