<!--
# license: Licensed to the Apache Software Foundation (ASF) under one
#         or more contributor license agreements.  See the NOTICE file
#         distributed with this work for additional information
#         regarding copyright ownership.  The ASF licenses this file
#         to you under the Apache License, Version 2.0 (the
#         "License"); you may not use this file except in compliance
#         with the License.  You may obtain a copy of the License at
#
#           http://www.apache.org/licenses/LICENSE-2.0
#
#         Unless required by applicable law or agreed to in writing,
#         software distributed under the License is distributed on an
#         "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
#         KIND, either express or implied.  See the License for the
#         specific language governing permissions and limitations
#         under the License.
-->

## Installation

    git clone https://github.com/sharh/cordova-plugin-yunba.git
    cordova plugin add cordova-plugin-yunba/com.bbk.plugins.push

## Methods

- `YunPush.setAlias(id, success, error);`
- `YunPush.start(id, success, error);`
- `YunPush.stop(id, success, error);`
- `YunPush.resume(id, success, error);`

    for more infomation visit : yunba.io.

## YunPush.setAlias
- id: as a user id.
- success: success callback
- error: error callback


### Example
    
    //yunba setAlias return msg
    function success(msg) {
        console.log(msg);
    }
    //plugin error
    function error(msg) {
        console.log(msg);
    }
    
    YunPush.setAlias('123456', success, error);

### Development mode
    
    you can change the YunPush.java file to make full js api.
    default the topic is 't1', change it to make yours.

### You must to set you appkey of yunba in plugin.xml.
    //change the str `your_yunba_appkey` to yours
-    <meta-data android:name="YUNBA_APPKEY" android:value="your_yunba_appkey" />


### Supported Platforms

- Android
