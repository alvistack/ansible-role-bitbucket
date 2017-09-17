Ansible Role for BitBucket
==========================

[![Build Status](https://travis-ci.org/alvistack/ansible-role-bitbucket.svg?branch=master)](https://travis-ci.org/alvistack/ansible-role-bitbucket)
[![GitHub tag](https://img.shields.io/github/tag/alvistack/ansible-role-bitbucket.svg)](https://github.com/alvistack/ansible-role-bitbucket)
[![GitHub license](https://img.shields.io/github/license/alvistack/ansible-role-bitbucket.svg)](https://github.com/alvistack/ansible-role-bitbucket/blob/master/LICENSE)

Ansible Role for Atlassian BitBucket Installation.

Requirements
------------

This role require Ansible 2.3 or higher.

This role was designed for Ubuntu 16.04/14.04 or CentOS 6/7.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>parameter</th>
<th>required</th>
<th>default</th>
<th>choices</th>
<th>comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>bitbucket_catalina</td>
<td>no</td>
<td><code>/opt/atlassian/bitbucket</code></td>
<td></td>
<td>Location for the BitBucket installation directory</td>
</tr>
<tr class="even">
<td>bitbucket_connector_port</td>
<td>no</td>
<td><code>7990</code></td>
<td></td>
<td>BitBucket Apache Tomcat connector port</td>
</tr>
<tr class="odd">
<td>bitbucket_context_path</td>
<td>no</td>
<td><code>~</code></td>
<td></td>
<td>Context path for BitBucket installation</td>
</tr>
<tr class="even">
<td>bitbucket_group</td>
<td>no</td>
<td><code>daemon</code></td>
<td></td>
<td>Name of the group that should own the file</td>
</tr>
<tr class="odd">
<td>bitbucket_home</td>
<td>no</td>
<td><code>/var/atlassian/application-data/bitbucket</code></td>
<td></td>
<td>Location for the BitBucket home directory</td>
</tr>
<tr class="even">
<td>bitbucket_jvm_maximum_memory</td>
<td>no</td>
<td><code>1024m</code></td>
<td></td>
<td>BitBucket JVM maximum memory usage</td>
</tr>
<tr class="odd">
<td>bitbucket_jvm_minimum_memory</td>
<td>no</td>
<td><code>512m</code></td>
<td></td>
<td>BitBucket JVM minimum memory usage</td>
</tr>
<tr class="even">
<td>bitbucket_jvm_support_recommended_args</td>
<td>no</td>
<td><code>-Datlassian.plugins.enable.wait=300</code></td>
<td></td>
<td>Atlassian Support recommended JVM arguments</td>
</tr>
<tr class="odd">
<td>bitbucket_owner</td>
<td>no</td>
<td><code>daemon</code></td>
<td></td>
<td>Name of the user that should own the file</td>
</tr>
<tr class="even">
<td>bitbucket_proxy_name</td>
<td>no</td>
<td><code>~</code></td>
<td></td>
<td>Domain name for working with reverse proxy</td>
</tr>
<tr class="odd">
<td>bitbucket_scheme</td>
<td>no</td>
<td><code>~</code></td>
<td><ul>
<li><code>http</code></li>
<li><code>https</code></li>
</ul></td>
<td>Scheme for working with reverse proxy</td>
</tr>
<tr class="even">
<td>bitbucket_server_port</td>
<td>no</td>
<td><code>8006</code></td>
<td></td>
<td>BitBucket Apache Tomcat server port</td>
</tr>
<tr class="odd">
<td>bitbucket_url</td>
<td>no</td>
<td><code>https://downloads.atlassian.com/software/stash/downloads/atlassian-bitbucket-5.3.1.tar.gz</code></td>
<td></td>
<td>URL for download archive</td>
</tr>
</tbody>
</table>

Dependencies
------------

No additional role dependencies.

Example Playbook
----------------

    - hosts: all
      roles:
        - role: bitbucket
          bitbucket_proxy_name: "bitbucket.example.com"
          bitbucket_scheme: "http"
          bitbucket_owner: "bitbucket"
          bitbucket_group: "bitbucket"

License
-------

-   Code released under [Apache License 2.0](https://github.com/alvistack/ansible-role-bitbucket/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

