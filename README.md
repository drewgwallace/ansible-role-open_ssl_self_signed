# Ansible Role

## Purpose
  Create Self Signed Certificate for easy continuity testing of deployments.

----

## Execution

<pre>
    - hosts: all
      tasks:
      - include_role:
          name: drewgwallace.openssl_self_signed
        vars:
          server_name: "<b>my_example</b>"
          server_url: "<b>url.example.com</b>"
</pre>

  ### Variables:
<pre>
# cert_common_name: certificate CN
# cert_country: certificate Country
# cert_email_address: the email address used in certificate
# cert_locality: certificate Locality
# cert_dir: the target directory that files will be output to
# cert_organizational_unit: certificate Organizational Unit
# cert_organization: certificate Organization
# cert_state: certificate State
# server_name: the name of the server (or otherwise) that will be utilizing the certificate
# force_regeneration: overwrite existing certificate files
# server_url: the URL used for CN and SAN identity

</pre>
----

## Notes