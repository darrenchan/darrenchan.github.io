============================
Austin OpenStack Summit 2016
============================

====================
Monday 25 April 2016
====================

ops-guide
~~~~~~~~~
 https://etherpad.openstack.org/p/PAO-ops-ops-guide-fixing
upgrades- work under different conditions, so the need to make it more generic.

Organising by services?

HA too much configuration detail, more abstract and conceptual information.
Don't document running supporting services like HAproxy etc.

Managing the cloud lifecycle
Troubleshooting out of date
Define
HP operations don't troubleshoot

Action:
Define the tasks operators want documented
Source downstream ops info to share upstream
email ops guide team on

Takeaways:
Share information upstream
Categorising information by persona causes duplication of information and makes information hard to find.
engaging with operators
Document real world experiences and what happens in production

Mitaka - Beyond the release notes
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Personas

Architect, Ops

Developers
Lead developer - managing users and policies
Domain Ops - in managed providers, managed SLAs. troubleshooting,

The Big Tent - One year later
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

What is it?

Projects moved from stack forge into an official projects
Benefits
- no longer stuck  - using governance to drive behaviour
- More collaboration between projects
- More reactivity - ideas are driven by users and operators and allowed creating of team
 - Competition - mechanisms to adding multiple projects to address the same problem
- Forced us to document the OpenStack way - project team guide
- Focus on the core infra

Disadvantages
Some projects are single vendor and remain that way.

Confusion between what we produce
It can be hard  for an established project to join OpenStack because of the governance requirements. For example, drop tools (e.g mailing list) and resources that works and is successful.\

Ugly
Cleaning up the tent


From Upstream Documentation To Downstream Product Knowledge Base
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Using Zendesk for support knowledge base content
Headings be more descriptive for SEO

================
Tuesday 26 April
================

Getting API docs off WADL and into RST
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

https://etherpad.openstack.org/p/newton-api-docs-rst

- fairy slipper generated website from swagger
- nova response requests are in the source tree, use testing samples
- parameters in yaml files
- Encourage projects to adopt best practices

HPE - Lifecycle Management of OpenStack using Ansible
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Deploy, reconfig, upgrade/upstre./hotfix, Add service to node, add/remove ode, offline/online nodes

- Conforming complexity - The number one barrier to enterprise adoption

- April 2016 User Survey Report
  Complexity - many choices to be made
  54 OpenStack projects

- Deployment considerations - OS, OpenStack

- Network configuration - flat, vlans, GRE tunnel, SDN

- Getting started with OpenStack page (7 options) vs Microsoft azure (1 option)

- Complexities - management

Address complexities
Docs -
User feedback 

fleet and inventory management

Installation Guide discussion
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- docs - revamping the install guide

- Need for comparison of deployment tools such as Fuel, ansible, etc to allow users to make a choice

- Each deployment has a reference architecture

OpenStack Talent development  - Lessons learned
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Community - embracing rookies
  An exam to measure the effectiveness of learning. 

- Teaching new developers to embrace the community culture and understand how
  to commit code, do code reviews, have a high degree of collaboration.

- Best way to learn is to teach it. All students will be adhoc professors and
   teach what they learned.
- Implemeent project deep dives
- Run classes to support technologies

OpenStack upgrades
~~~~~~~~~~~~~~~~~~

- Isolation is important for rollbacks
- QA is invaluable after testing upgrade
- Co-gating jobs will test for each service
- Control plane
- open window for customers to test

Why is it a problem for customers to upgrade to current releases?
- Upgrades are hard, lose connectivity for a period of time
- We don't necessarily need new features, hence don't upgrade
nova

- 45 minutes for database migration
- no planning necessary with Cola container
- How long does it take to do upgrade? Outage? Control plane changes is not
  outage time.

==================
Wednesday 27 April
==================

API docs session
~~~~~~~~~~~~~~~~

API Guides https://etherpad.openstack.org/p/austin-docs-workgroup-api


OpenStack Ansible - Ubuntu 16.04 Preparation
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

https://etherpad.openstack.org/p/openstack-ansible-newton-ubuntu16-04

Ubuntu 16.04 support in conjunction with Ubuntu 14.04 support

 - Getting system.d up and running
 - Already addressed package name differences
 - Submit a review to propose a pattern (?)
 - Approach: Template the compute node as a separate operating system install
 - Problem getting infrastructure running on 16.04
 - Percona back up solution is a blocker for 16.04. Importing packages does not work
 - Possible option to install packages from distro
 - Focus on priorities rather than addressing requests for new features
 - Support multiple ??
 
Mitaka retrospective
~~~~~~~~~~~~~~~~~~~~
 https://etherpad.openstack.org/p/austin-docs-mitakaretro

Installation Guide
~~~~~~~~~~~~~~~~~~

https://review.openstack.org/#/c/301284
https://etherpad.openstack.org/p/austin-docs-workgroup-install

Action item
-----------
- Liaise with Mike Perez (thingee), Christian on establishing a project
  install guide template.
  
  
OpenStack Ansible docs
~~~~~~~~~~~~~~~~~~~~~~

https://etherpad.openstack.org/p/openstack-ansible-newton-role-docs

- Ownership with developers
- Working group with technical lead - Darren, Robb, Alex, Major, Travis, Amy, 

=================
Thursday 28 April
=================

Contributor Guide
~~~~~~~~~~~~~~~~~

https://etherpad.openstack.org/p/austin-docs-contributorguide

Action items
------------
- Mailing list and working group to establish standards/tooling for diagrams

Security Guide
~~~~~~~~~~~~~~
https://etherpad.openstack.org/p/austin-docs-workgroup-security 
- Neutron content out of date

Networking guide
~~~~~~~~~~~~~~~~

https://etherpad.openstack.org/p/austin-docs-workgroup-networking

Ops-guide has architecture scenarios that should reference the networking-guide


Docs Newton planning
~~~~~~~~~~~~~~~~~~~~
https://etherpad.openstack.org/p/austin-docs-newtonplan

===============
Friday 29 April
===============

Docs contributors meetup
~~~~~~~~~~~~~~~~~~~~~~~~

- Discussion with Shaun O'Meara and Robert Starmer on ops-guide and arch-guide
- Revised arch-guide TOC and ops-guide edits
  https://etherpad.openstack.org/p/ops-arch-tasks
- Deprecated mitaka arch-guide spec and drafted newton arch-guide spec
  https://blueprints.launchpad.net/openstack-manuals/+spec/arch-guide-restructure

======================
Summit follow up tasks
======================

- Confirm action items with specialty team
- Develop delivery plan for ops-guide
- Establish ops tasks on etherpad / mailing list
- Audit ops guides
- Enquire about Rackspace internal ops content
- Follow up on Comcast (Shilla), Rackspace (Melvin Hillsman) and HPE (Joel) provide ops content
- Check for open source licensing for lucidchart (Shaun)
- Install guide project template

arch guide discussion with Shaun O'meara

- abstraction layer approach
- develop a task list

Ops Guide
- Specifics on performing backups

