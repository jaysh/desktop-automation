desktop-automation
==================

Ansible scripts that I run in order to convert a basic apt based distribution into a useful development/desktop environment for me.

# How to use it

1. Clone this repository (see right side of the page)
2. Run `sudo ansible-playbook -c local -i '127.0.0.1,' site.yml `
3. ???
4. Profit!

# Things left to do

In general, now this is an unscalable set of scripts that configure a personal laptop or desktop into a setup I'm comfortable with. Lots of assumptions are made: every environment should be the same, and anyone else who uses this repository wants exactly the same packages as I do. Right now, this is true for me, which is why it's this way. However, this is just a starting point for people to tell me what they'd like different so I can take those thoughts on board. I have lots of things in the pipeline that I plan:

- Using `etckeeper` properly to manage my `/etc`
- Automated nightly incremental backups of my laptop either via `rsync`, `obnam` or something even more awesome
- Checking out such a backup when deploying a new operating system
- Configuring Chrome with my Google Account (probably not worth doing)
- Automatically wiping my laptop every month, and network installing the latest build of my favourite distribution, and running all of these scripts including restoring my home directory (it's a strange dream)
