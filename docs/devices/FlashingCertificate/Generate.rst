.. _devices-provisioning-certificate-generate:

Generating a certificate
########################

You can use the CLI to generate a certificate for your device.
The firmware will use the IMEI of the device as the MQTT client ID.
You can get the IMEI of your device using the AT command ``AT+CGSN``.

Following is the output of the command:

.. code-block::

    352656100248049 OK

Use the IMEI when generating the certificate:

.. code-block:: bash

    node cli create-device-cert -d "<imei>"
