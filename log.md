# 100 Days Of Code - Log

### Day 0: Thursday, January 5, 2017

**Today's Progress**

* Explored deeper into nix and `nixpkgs.nodePackages`
* Set up Kik chat wrapper for chatwithbenz

**Thoughts**

* Nix makes sense
* Kik bots are really easy to start working with, but the documentation doesn't seem to cover setting up ngrok with the bot server.

**What I learned**

* `nix-env -f '<nixpkgs>' -iA nodePackages.some_package` installs `some_package` from `nodePackages`. A list of available Node packages in Nix can be found [here](https://github.com/NixOS/nixpkgs/blob/master/pkgs/top-level/node-packages.json). [Source](https://github.com/svanderburg/node2nix)
* Example: adding a node package to nix [yarn PR](https://github.com/NixOS/nixpkgs/pull/20635).
* Update nix channel with `nix-channel --update`

**Link(s) to work**

* I'm keeping `chatwithbenz` local until it actually does something.
