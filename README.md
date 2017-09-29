# redfish-client-node
Redfish 1.0 Node.js client library 

Copyright © 2017 Dell Inc. or its subsidiaries.  All Rights Reserved. 

## Getting Started
See example.py for usage examples.

## Generating code
```
sudo apt-get install -y maven
git clone https://github.com/RackHD/on-http.git
git clone https://github.com/swagger-api/swagger-codegen.git
pushd ./swagger-codegen && mvn package && popd
java -jar ./swagger-codegen/modules/swagger-codegen-cli/target/swagger-codegen-cli.jar \
  generate -i on-http/static/redfish.yaml -o redfish-client-node -l javascript
```

## Licensing

Licensed under the Apache License, Version 2.0 (the “License”); you may not use this file except in compliance with the License. You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an “AS IS” BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.

RackHD is a Trademark of Dell EMC
