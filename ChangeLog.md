# Change Log

## v0.6

Highlights:

* Defaults to downloading latest stemcell (rather than stable, which are getting old now).
* Installs the Cloud Foundry plugin for BOSH https://github.com/StarkAndWayne/bosh-cloudfoundry

Additions:

* `tmux` - if you have tmux installed, then you can SSH into inception VM with it (thx @mrdavidlang)
* started a test suite; its small but growing! (thx @mrdavidlang for getting it started)

Bug fixes:

* Fog::SSH uses explicit ssh key that was requested to access inception VM

Future thoughts:

* I hate Settingslogic for read-write settings. It's really only a read-only settings DSL. It puts Ruby classes into the YAML. Probably going to rip it out.
* I am so sorry I took so long to start writing tests. It always seemed such a hard thing to write tests for. But bosh-cloudfoundry project has had good success with internal tests; so we're migrating those ideas into this project.