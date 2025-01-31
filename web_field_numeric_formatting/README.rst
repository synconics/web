============================
Web Numeric Field Formatting
============================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-LGPL--3-blue.png
    :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
    :alt: License: LGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fweb-lightgray.png?logo=github
    :target: https://github.com/OCA/web/tree/16.0/web_field_numeric_formatting
    :alt: OCA/web
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/web-16-0/web-16-0-web_field_numeric_formatting
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/162/16.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

Having this module installed allows a developer to render a float or integer field
without a thousands separator using

.. code-block:: xml

   <field name="id" options="{'enable_formatting': false}" />

Setting this option is supported for list and form views. In kanban views you
can simply use

.. code-block:: xml

    <t t-esc="record.id.raw_value" />

The code in this module is a backport of
https://github.com/odoo/odoo/commit/592794b397ba7f6468e45a5cc3e93681b1ed8578
from Odoo 17, so this module should not be ported beyond version 16.

The new `enable_formatting` option in Odoo 17 replaces the `format` option in
Odoo 15.

**Table of contents**

.. contents::
   :local:

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/web/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/web/issues/new?body=module:%20web_field_numeric_formatting%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Opener B.V.

Contributors
~~~~~~~~~~~~

* Lucas Perais (lpe) <lpe@odoo.com> contributed the original code to Odoo.
* Stefan Rijnhart <stefan@opener.amsterdam> created the backport to Odoo 16
  in this module.

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/web <https://github.com/OCA/web/tree/16.0/web_field_numeric_formatting>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
