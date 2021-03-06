==============================
Web Based Management Console
==============================

Please reference the "CentreStack Admin Guide" for more details about tenant administration.
Here is a few points that are more important during the deployment phase.

You can enter the web based management console by selecting ‘Management Console’ under user’s
name in the top right.

.. image:: _static/image044.png

After you click into the "Management Console", you will see tenant level management 
tasks.

.. image:: _static/image044_1.png


Team Folders
^^^^^^^^^^^^^^

Team Folders are created by the tenant admin. The users that can be assigned to the team folders are the team users
within the tenant. Each team user can be assigned read or write permissions to the team folder. For the team
users that are not assigned with a specific team folder, the team folder will not show up.
Team folders users can also be assigned the “Owner” permission. The owner permission allows the “owner” to
maintain and manage the team folder permissions.

.. image:: _static/image045.png

Storage Manager
^^^^^^^^^^^^^^^^^

Tenant admin can update the default (primary) storage configuration information. For example, if the default
storage is using Amazon S3, the tenant admin can update the S3 bucket, access key and secret key. However,
tenant admin can not switch the default storage into a different storage service. The cluster
admin can help the tenant admin switch the default storage.

Tenant admin can also add auxiliary storage by using the “Attach Storage”
options. Default storage is the root folder of the tenant. Attached auxiliary storage is top level folders
inside the root folder.

.. image:: _static/image046.png

User Manager
^^^^^^^^^^^^^^^^

In user manager, you can create users, import users from Active Directory over LDAP or import users from
Active Directory via Server Agent.

.. image:: _static/image047.png

.. image:: _static/image048.png


Delegate Administration
^^^^^^^^^^^^^^^^^^^^^^^^^

You can add full delegated admin to the list of “Cloud Administrators”.

.. image:: _static/image050.png

Active Directory Integration (Optional)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

It is optional to setup Active Directory Integration. You can get to the integration page from
Management Console -> Advanced -> Active Directory Settings. The active directory setting
here refers to local Active Directory with LDAP integration. For remote Active Directory, server
agent can be used to connect remote file server folders and remote Active Directory.

.. image:: _static/image051.png

.. note::

    If this specific tenant's Active Directory is at a remote location, please
    use CentreStack Server Agent to connect Active Directory (No need to use
    LDAP over Internet WAN connection).

Group Policy
^^^^^^^^^^^^^^

Granular group policies can be configured for the entire tenant users from Management Console -> Group Policy.

.. image:: _static/image052.png


Please reference "CentreStack Admin Guide" for complete reference for tenant administration.