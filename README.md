Virtualmin Cookbook
===================
Installs or configures the Virtualmin server control panel. http://www.virtualmin.com/

Requirements
------------
Chef 11

Requires `selinux` [cookbook](http://community.opscode.com/cookbooks/selinux) on RHEL Family

Platform
--------
* CentOS, Red Hat

Tested on:

* CentOS 6.3

Attributes
----------

<table>
  <tr>
    <th>Key</th>
    <th>Type</th>
    <th>Description</th>
    <th>Default</th>
  </tr>
  <tr>
    <td><tt>['virtualmin']['serial_number']</tt></td>
    <td>String</td>
    <td>Serial Number</td>
    <td><tt>GPL</tt></td>
  </tr>
  <tr>
    <td><tt>['virtualmin']['license_key']</tt></td>
    <td>String</td>
    <td>License Number</td>
    <td><tt>GPL</tt></td>
  </tr>
</table>

Usage
-----

Just include `virtualmin` in your node's `run_list`:

```json
{
  "name":"my_node",
  "run_list": [
    "recipe[virtualmin]"
  ]
}
```

Contributing
------------

1. Fork the repository on Github
2. Create a named feature branch (like `add_component_x`)
3. Write you change
4. Write tests for your change (if applicable)
5. Run the tests, ensuring they all pass
6. Submit a Pull Request using Github

License and Authors
-------------------
Authors: Steven Barre (<steven@realestatewebmasters.com>)

Copyright 2013, Steven Barre

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
