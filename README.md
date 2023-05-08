Role Name
=========

This will setup and prep a host to be a ssv node.

Requirements
------------

Ubuntu 22.04 LTS

Role Variables
--------------

  BeaconNodeAddr: "prater-4000-ext.stage.bloxinfra.com:80"
    This is a beacon chain end point.

  ETH1Addr: "ws://eth1-ws-ext.stage.bloxinfra.com/ws"
    ws eth end point to query and subscribe to.

  RegistryContractAddr: "0x687fb596F3892904F879118e2113e1EEe8746C2E"
    Please verify this address before using.

  network_name: "prater"
    The network name for the config.yaml.

  data_path: "/var/lib/"
    Where the data should be stored.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: ssv-validator
          BeaconNodeAddr: "prater-4000-ext.stage.bloxinfra.com:80"
          ETH1Addr: "ws://eth1-ws-ext.stage.bloxinfra.com/ws"

License
-------

BSD

Author Information
------------------

Frazz from STKD.io