.. title:: Nutanix Calm Windows Workshop

.. toctree::
  :maxdepth: 2
  :caption: Calm and Windows
  :name: _calm_and_windows
  :hidden:

  what_is_calm/what_is_calm
  calm_win/calm_win

.. toctree::
  :maxdepth: 3
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

Access Instructions
+++++++++++++++++++

The Nutanix Hosted POC environment can be accessed a number of different ways:

Please use install a VPN client (faster) to connect to the remote lab in US. https://xlv-uswest1.nutanix.com/

Or, using a HTML5 VDI (slower) to connect to the remote lab in US. https://xld-uswest1.nutanix.com/

You should have one page of lab access info. If you don’t, please seek help from your instructor.

If you have any questions, please feel free to ask.

..............................

**Username:** POCxxx-User01 (up to POCxxx-User20), **Password:** *customerSE/4u*

Under **Client Application Sessions**, click **Start** to the right of **Pulse Secure** to download the client.


Hosted POC clusters follow a standard naming convention:

- **Cluster Name** - POC\ *XYZ*
- **Subnet** - 10.42.**.\ *XYZ*\ .0
- **Cluster IP** - 10.42.**.\ *XYZ*\ .37

If provisioned from the marketing pool:
- **Cluster Name** - MKT\ *XYZ*
- **Subnet** - 10.41.**.\ *XYZ*\ .0
- **Cluster IP** - 10.41.**.\ *XYZ*\ .37

For example:

- **Cluster Name** - POC055
- **Subnet** - 10.42.50.0
- **Cluster IP** - 10.42.50.37

Throughout the Workshop there are multiple instances where you will need to substitute *XYZ* with the correct octet for your subnet, for example:

.. list-table::
   :widths: 25 75
   :header-rows: 1

   * - IP Address
     - Description
   * - 10.42.**.37
     - Nutanix Cluster Virtual IP
   * - 10.42.**.39
     - **PC** VM IP, Prism Central
   * - 10.42.**.51
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
     - customerSE/4u
   * - Prism Central
     - admin
     - customerSE/4u
