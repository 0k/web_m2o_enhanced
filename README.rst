==================================
Add new options for many2one field
==================================


Description
-----------

This modules modifies "many2one" form fields so as to add some new display
control options.

Options provided includes possibility to remove "Create..." and/or "Create and
Edit..." entries from many2one drop down. You can also change default number of
proposition appearing in the drop-down. Or prevent the dialog box poping in
case of validation error.

Please note that the default behavior of this module is to match the default
OpenERP behavior.


Requirements
------------

Was tested on openerp v7.0


New option
----------

``create`` *boolean* (Default: ``true``)

  Whether to display the "Create..." entry in dropdown panel.

``create_edit`` *boolean* (Default: ``true``)

  Whether to display "Create and Edit..." entry in dropdown panel

``limit`` *int* (Default: openerp default value is ``7``)

  Number of displayed record in drop-down panel

``m2o_dialog`` *boolean* (Default: ``True``)

  Whether to display the many2one dialog in case of validation error.

Example
-------

Your XML form view definition could contain::

    ...
    <field name="partner_id" options="{'limit': 10, 'create': false, 'create_edit': false}"/>
    ...

