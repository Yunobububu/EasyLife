# StarUML 安装与破解for mac
- 安装StarUML [http://staruml.io/download]
- 修改 LicenseManagerDomain.js 默认安装目录为(可以在终端用(`find / -name LicenseManagerDomain.js`命令查找)：
- /Applications/StarUML.app/Contents/www/license/node/LicenseManagerDomain.js
```
(function () {
    "use strict";

    var NodeRSA = require('node-rsa');

    function validate(PK, name, product, licenseKey) {
        var pk, decrypted;
        //添加以下代码
        return {
          name:"Oxcb",
          product:"StarUML",
          LICENSEType:"vip",
          quanlity:"mergades.com",
          licenseKey:"later equals never!"
        };
        try {
            pk = new NodeRSA(PK);
            decrypted = pk.decrypt(licenseKey, 'utf8');
        } catch (err) {
            return false;
        }
        var terms = decrypted.trim().split("\n");
        if (terms[0] === name && terms[1] === product) {
```
- 保存退出
- StarUML -> help -> Enterlicense -> Oxcb -> OK
