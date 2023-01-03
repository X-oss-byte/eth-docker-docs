---
id: BeforeYouStart
title:  Before you start.
sidebar_label: Before you start
---

Warnings about the dangers of running Ethereum staking full nodes are in [Recommendations.md](../Support/Recommendations.md).
In particular, you must be sure to secure your seed phrase, the mnemonic. You need it to recreate keys, and
to set a withdrawal address, if you didn't already do so during key creation.

You may also want to take a look at a [guide to Linux host security](https://www.coincashew.com/coins/overview-eth/guide-or-security-best-practices-for-a-eth2-validator-beaconchain-node#setup-two-factor-authentication-for-ssh-optional).

## eth-docker configuration wizard

A simple config wizard is included, and is briefly described in Step 2.

The same script can also be used to stop, start and update the node. Run `./ethd` for a help screen.

## eth-docker setup

1. Install prerequisites
2. Choose a client and do initial security setup.
3. Generate deposit files and an eth wallet. This can be done within this project, or outside of it
4. Import the validator keystore files generated in the previous step
5. Run the client
6. Finalize the deposit. This is not done within this project
7. A baseline set of Grafana dashboards are included.  Feel free to add more, or submit a PR with your favorite dashboards.
8. Configure your system to automatically prune Geth (optional)

> The documentation does not show `sudo` for docker commands. If your user is not part of the `docker` group, you will need `sudo`. For example, `sudo docker ps` instead of just `docker ps`. This guide shows you how to add your user account to the `docker` group in step 2.
