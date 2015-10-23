

DESCRIPTION
--
This is the forked version of the vcloud-rest from https://github.com/vmware/vcloud-rest. It's forked to add more functionality for the Rest API's. 

Example:
 1. Ability to create a stand alone vApp Network 
 2. Ability to create vApp Network with DHCP enabled.
 3. Ability to compose entire vApp in one pass instead of adding VM to vApp one by one.
 4. Ability to create a VM with nic disconnected and more.

 Will be adding more changes slowly.


PREREQUISITES
--
- nokogiri
- rest-client
- httpclient
- ruby-progressbar


USAGE
--

    require 'vcloud-rest/connection'
    conn = VCloudClient::Connection.new(HOST, USER, PASSWORD, ORG_NAME, VERSION)
    conn.login
    conn.get_organizations

EXAMPLE
--
A (mostly complete) example can be found in

    examples/example.rb



LICENSE
--

Author:: Stefano Tortarolo <stefano.tortarolo@gmail.com>

Copyright:: Copyright (c) 2012-2015
License:: Apache License, Version 2.0

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

CREDITS
--
This code was inspired by [knife-cloudstack](https://github.com/CloudStack-extras/knife-cloudstack).
