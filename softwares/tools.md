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

# [brew](https://brew.sh/) 安装for Mac
* 打开终端
* 复制命令
* `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
* 可能会询问创建新的文件夹,确认即可
