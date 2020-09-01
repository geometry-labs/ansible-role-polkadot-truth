polkadot-truth
=========

This role prepares the node for installation of the Polkadot client as a source of truth node.

Role Variables
--------------

### Sync

- aws_access_key_id: none
- aws_secret_access_key: none
- region: us-east-1
- sync_bucket_uri: none
- chain_stub: polkadot

### Polkadot Client

- project: default
- chain: polkadot
- loggingFilter: "sync=trace,afg=trace,babe=debug"
- telemetryUrl: none

Dependencies
------------

- w3f_insight.polkadot_base

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: insight_w3f.polkadot_truth }

License
-------

Apache 2.0

Author Information
------------------

Maintained by [Richard Mah](https://github.com/shinyfoil) for [Insight Infrastructure](https://github.com/insight-infrastructure)
