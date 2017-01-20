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


### Day 1: Friday, January 6, 2017

**Today's Progress**

Uh oh, went on a flight from Kelowna to Toronto today. It was supposed to leave in the morning but got delayed to past noon. By the time I arrive and get to my Airbnb, it was already time for bed. Hackthon tomorrow, will try harder then.


### Day 2 & 3: Saturday, January 7, 2017 and Sunday, January 8, 2017

**Progress**

* Went to [HackTheValley](https://www.hackvalley.com/), played with Amazon Echo, and made a [custom Skill](https://devpost.com/software/alexa-my-personal-therapist) for it.

**What I learned**

* How to make an Alexa Skill in Javascript using [alexa-app](https://github.com/matt-kruse/alexa-app) and serve it using [alexa-app-server](https://github.com/matt-kruse/alexa-app-server).
* Strengthened my knowledge in basic reinforcement learning through designing a language interface that correctly understands user sentiments and provides accurate, appropriate feedback.

**Link(s) to work**

* [Alexa: My Personal Therapist](https://devpost.com/software/alexa-my-personal-therapist)


### Day 4: Monday, January 9, 2017

**Progress**

* Took a day off before the first day of work for life stuff.


### Day 5: Tuesday, January 10, 2017

**Progress**

* Confidential work-related things. Read a lot of documentation and code.
* Set up zprezto on work computer.


### Day 6: Wednesday, January 11, 2017

**Progress**

* Work-related: Python ndb and protobuf + Google App Engine

*Oops, got carried away with life. Let's restart.*

### Day 0: Sunday, January 15, 2017

**What I did**

* A command-line utility that automatically manages `.gitignore` files

**Thoughts**

* It takes a lot of effort to polish an app, even with small scripts.

**Link(s) to work**

* Still WIP, implemented the add functionality but not the remove. Also it doesn't yet check for duplicates.

### Day 1: Monday, January 16, 2017

**What I did**

* Learned how to contribute to [nixpkgs](https://github.com/NixOS/nixpkgs).
* Bumped [Yarn][yarn] from [v0.18.1 to v0.19.1][nixpkgs-pull-21945] in nixpkgs.

**Thoughts**

* Nix is learnable, if we dig deep enough. It appears to have a very steep learning curve, but after getting over that, everything seems to make more sense. It is important to read the official docs carefully, most of it is very well written.

**What I learned**

* [Yarn][yarn] is now a top-level package as of [yarn: init at 0.18.1](https://github.com/NixOS/nixpkgs/pull/21892)
* To install yarn: `nix-env -iA nixpkgs.yarn`

**Link(s) to work**

* [NixOS/nixpkgs#21945][nixpkgs-pull-21945]

[nixpkgs-pull-21945]: https://github.com/NixOS/nixpkgs/pull/21945
[yarn]: https://github.com/yarnpkg/yarn

### Day 2: Tuesday, January 17, 2017

**What I did**

* Received my Kickstarter-backed [Onion Omega 2+][omega2-kickstarter] in the mail today. Played around with it and Read through its [documentation](https://docs.onion.io/omega2-docs/). Didn't get the serial connection to work, but Wifi and AP both work out-of-the-box. AP sometimes crashes.

<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052232/096a5cd0-dd17-11e6-9170-9e28b405d749.jpg" />
<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052152/9b3aa774-dd16-11e6-8c2a-a72d2f50a849.jpg" />
<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052153/9b3de498-dd16-11e6-9169-60a6aeb8d6b6.jpg" />
<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052149/9b39d222-dd16-11e6-8b5f-48c70dac064a.jpg" />
<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052151/9b3a7aa6-dd16-11e6-8006-d4844b0eb516.jpg" />
<img width="16%" src="https://cloud.githubusercontent.com/assets/5977478/22052150/9b39ee74-dd16-11e6-9848-b055ac3f550c.jpg" />

**What I learned**

* Omega2+ currently uses the [Dropbear SSH][dropbear], which is supposed to have "a small memory footprint" and is suitable for IOT devices.
* Omega2+ has a 580MHz CPU, 128MB Memory, and 32MB storage, which is a lot less compared to Raspberry Pi. This is probaby because it's more targeted toward the hardware side of things (it's like Raspberry Pi and Arduino had a child).

[omega2-kickstarter]: https://www.kickstarter.com/projects/onion/omega2-5-iot-computer-with-wi-fi-powered-by-linux
[dropbear]: https://matt.ucc.asn.au/dropbear/dropbear.html

### Day 2: Wednesday, January 18, 2017

**What I did**

* A lot of work on [IgnoreMe][ignoreme] (used to be IgnoreIt, but apparently someone took that name on npm) to get the MVP published today.
* Took a really quick look at ESLint.

**Thoughts**

* Eslint is pretty cool, but without reading through the docs I can't figure out how to properly customize the rules. I'll read the docs when I encounter it the next time.
* A lot of people made `.gitignore` automation scripts, but none of them seem to be polished for pleasant everyday usage.

**What I learned**

* Always overestimate the amount of time needed to complete a software project. I (once again) thought it'd take an hour to finish up IgnoreMe since progress from two days ago, but it took 5 hours...

**Links to work**

IgnoreMe on [Github][ignoreme] and [NPM][ignoreme-npm]

[ignoreme]: https://github.com/ben-z/ignoreme
[ignoreme-npm]: https://www.npmjs.com/package/ignoreme

### Day 3: Thursday, January 19, 2017

**What I did**

* Stayed late at work to push a pretty large change. Heading to PennApps tonight.

**What I learned**

Google App Engine's datastore explicitly checks for the type of `datetime` when executing a query, which makes `freezegun.greeze_time` unusable:

```
BadValueError: Unsupported type for property created_at: <class 'freezegun.api.FakeDatetime'>
```

A workaround is to patch GAE internals, as outlined [here](https://nvbn.github.io/2016/04/14/gae-datastore-freeze-time/):

```python
from contextlib import contextmanager
from google.appengine.api import datastore_types
from mock import patch
from freezegun import freeze_time as _freeze_time
from freezegun.api import FakeDatetime


@contextmanager
def freeze_time(*args, **kwargs):
    with patch('google.appengine.ext.db.DateTimeProperty.data_type',
                new=FakeDatetime):
        datastore_types._VALIDATE_PROPERTY_VALUES[FakeDatetime] = \
            datastore_types.ValidatePropertyNothing
        datastore_types._PACK_PROPERTY_VALUES[FakeDatetime] = \
            datastore_types.PackDatetime
        datastore_types._PROPERTY_MEANINGS[FakeDatetime] = \
            datastore_types.entity_pb.Property.GD_WHEN
            
        with _freeze_time(*args, **kwargs):
            yield
```
