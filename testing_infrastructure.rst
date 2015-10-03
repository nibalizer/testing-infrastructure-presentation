.. transition:: tilt
   :duration: 0.4

Testing Infrastructure
======================
.. transition:: tilt

Spencer Krum

* Engineer at IBM
* Former CAT
* OpenStack and Puppet contributor 
* @nibalizer on pretty much everything

OpenStack Infra
===============
.. transition:: tilt

Brief Overview

Agenda
======
.. transition:: tilt

* High level theory
* What to test
* How to test

Perspectives
============
.. transition:: tilt


* App developer
* Operator
* Net Engineer

Layers
======
.. transition:: tilt


* Physical
* Cloud resources
* Server configuration
* Services

Infrastructure is not static
============================
.. transition:: tilt

* Things we touched
* Things we didn't touch
* Things we created

Testing won't be static either
==============================
.. transition:: tilt

* Polling test
* Infrequent test
* Post-action test

You can't test everything
=========================
.. transition:: tilt

There isn't time


Risk Mgmt
=========
.. transition:: tilt
.. code:: python

   Probability vs Impact

     +-----+-----+
     |     |     |
   ^ |     |     |
   | | med | crit|
   p +-----+-----+
     |     |     |
     |     |     |
     | low | high|
     +-----+-----+
        i ->


Things that don't work
======================

* Staging Environment
* Heavy integration tests


Testing
=======

* Learn from Developers
* VCS all the things
* Run lint/syntax
* Code review everything
* break code into chunks, test those


Techniques
==========

* set -e


Techniques
==========

* Serverspec w/ Packer or dib


Techniques
==========

* Canary Deploy


Techniques
==========

* Beaker, beaker-rspec, serverspec

Techniques
==========

* puppet agent --test --noop
* puppet agent --test --environment=mytestenv


Techniques
==========

* Cloudformation, Terraform, Ansible


Techniques
==========

* Integration tests for libraries


Summary
=======

* Test where the risk is
* Break infra into chunks, test those
* Follow the patterns from developers
* Be aware of the infra underneath you
* Code review everything


Questions
=========
.. transition:: tilt

Spencer Krum

* Engineer at IBM
* Former CAT
* OpenStack and Puppet contributor 
* @nibalizer on pretty much everything

