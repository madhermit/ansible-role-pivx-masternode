## after daemon starts it needs to sync the block chain.
When done with synchronisation, the RequestedMasternodeAssets field must be 999:

    $ ./pivx-cli mnsync status | grep RequestedMasternodeAssets

Alternatively, you can see what block its syched up to so far:

    $ ./pivx-cli getinfo | grep blocks

## Start the masternode on your local wallet (make sure masternode ips match)

    $ startmasternode "alias" "0" "<masternode alias>"

## Check the status of the masternode

    $ ./pivx-cli masternode status

## Starting the PIVX daemon (if its not started by the playbook)

    $ ./pivxd -daemon

## Stopping the PIVX daemon

    $ ./pivx-cli stop

## Official Guide

    https://pivxmasternode.org/2017/03/08/step-step-guide-setting-masternode/

## Credits

    https://forum.pivx.org/t/vultr-com-ubuntu-16-04-64bit-masternode-setup-guide/349
    https://steemit.com/pivx/@bm842/setup-a-pivx-masternode-on-linux
    https://pivx.freshdesk.com/support/solutions/articles/30000021125-using-the-bootstrap


## TODO

Add support for daily snapshots `http://178.254.23.111/%7Epub/PIVX/Daily-Snapshots-Html/PIVX-Daily-Snapshots.html`
