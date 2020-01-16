.. title:: Nutanix Calm Windows Workshop

.. toctree::
  :maxdepth: 2
  :caption: Calm and Windows
  :name: _calm_and_windows
  :hidden:

  what_is_calm/what_is_calm
  calm_win/calm_win

.. toctree::
  :maxdepth: 2
  :caption: Appendix
  :name: _appendix
  :hidden:

  appendix/glossary
  appendix/basics
.. _getting_started:

---------------
Getting Started
---------------

Welcome to the Nutanix Calm Windows Workshop! This workbook accompanies an instructor-led session that introduces Nutanix solutions and many common management tasks. Each section has a lesson and an exercise to give you hands-on practice. The instructor explains the exercises and answers any additional questions that you may have.

At the end of the bootcamp, attendees should understand the basic concepts and technologies that make up the Nutanix Enterprise Cloud stack and should be well prepared for a hosted or onsite proof-of-concept (POC) engagement.

What's New
++++++++++

- Workshop updated for the following software versions:
    - AOS & PC 5.10.x

- Optional Lab Updates:


Agenda
++++++

- Introductions
- Nutanix Calm

Introductions
+++++++++++++

- Name
- Familiarity with Nutanix

Initial Setup
+++++++++++++

- Take note of the *Passwords* being used.
- Log into your virtual desktops (connection info below)

Environment Details
+++++++++++++++++++

Nutanix Workshops are intended to be run in the Nutanix Hosted POC environment. Your cluster will be provisioned with all necessary images, networks, and VMs required to complete the exercises.

Networking
..........

Hosted POC clusters follow a standard naming convention:

- **Cluster Name** - POC\ *XYZ*
- **Subnet** - 10.**41**.\ *XYZ*\ .0
- **Cluster IP** - 10.**41**.\ *XYZ*\ .37

If provisioned from the marketing pool:
- **Cluster Name** - MKT\ *XYZ*
- **Subnet** - 10.**41**.\ *XYZ*\ .0
- **Cluster IP** - 10.**41**.\ *XYZ*\ .37

For example:

- **Cluster Name** - POC055
- **Subnet** - 10.41.55.0
- **Cluster IP** - 10.41.55.37

Throughout the Workshop there are multiple instances where you will need to substitute *XYZ* with the correct octet for your subnet, for example:

.. list-table::
   :widths: 25 75
   :header-rows: 1

   * - IP Address
     - Description
   * - 10.41.\ *XYZ*\ .37
     - Nutanix Cluster Virtual IP
   * - 10.41.\ *XYZ*\ .39
     - **PC** VM IP, Prism Central
   * - 10.41.\ *XYZ*\ .40
     - **DC** VM IP, NTNXLAB.local Domain Controller


Credentials
...........

.. note::

  The *<Cluster Password>* is unique to each cluster and will be provided by the leader of the Workshop.

.. list-table::
   :widths: 25 35 40
   :header-rows: 1

   * - Credential
     - Username
     - Password
   * - Prism Element
     - admin
     - *<Cluster Password>*
   * - Prism Central
     - admin
     - *<Cluster Password>*
   * - Controller VM
     - nutanix/4u
     - *<Cluster Password>*
   * - Prism Central VM
     - nutanix/4u
     - *<Cluster Password>*

Each cluster has a dedicated domain controller VM, **DC**, responsible for providing AD services for the **NTNXLAB.local** domain. The domain is populated with the following Users and Groups:

.. list-table::
   :widths: 25 35 40
   :header-rows: 1

   * - Group
     - Username(s)
     - Password
   * - Administrators
     - Administrator
     - nutanix/4u
   * - SSP Admins
     - adminuser01-adminuser25
     - nutanix/4u
   * - SSP Developers
     - devuser01-devuser25
     - nutanix/4u
   * - SSP Power Users
     - poweruser01-poweruser25
     - nutanix/4u
   * - SSP Basic Users
     - basicuser01-basicuser25
     - nutanix/4u

Access Instructions
+++++++++++++++++++

The Nutanix Hosted POC environment can be accessed a number of different ways:

Parallels VDI
.............

Login to https://xld-uswest1.nutanix.com (for PHX) or https://xld-useast1.nutanix.com (for RTP) using your supplied credentials

Select HTML5 (web browser) OR Install the Parallels Client

Select a desktop or application of your choice.

Pulse Secure VPN
..........................

https://sslvpn.nutanix.com - Use your CORP credentials

Pulse Secure VPN
..............................

https://xlv-uswest1.nutanix.com/ - **Username:** POCxxx-User01 (up to POCxxx-User20), **Password:** *customerSE/4u*

Under **Client Application Sessions**, click **Start** to the right of **Pulse Secure** to download the client.
