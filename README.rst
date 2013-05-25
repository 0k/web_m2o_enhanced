===================================
Add new options for many2one field:
===================================

- create: true/false -> disable "create" entry in dropdown panel 
- create_edit: true/false -> disable "create and edit" entry in dropdown panel
- limit: 10 (int) -> change number of selected record return in dropdown panel
- m2o_dialog: true/false -> disable quick create M20Dialog triggered on error.

Example:
--------

<field name="partner_id" options="{'limit': 10, 'create': false, 'create_edit': false}"/>

Note:
-----

if one of those options are not set, many2one field use default many2one field options.

