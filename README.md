# This project is for demonstration purposes only. 

 - It is for those who are interested in building a Backend system to test how client apps connect to such system. By this way, they can further write backend code for their own business, meeting their own needs. 
 - This demonstration project offers main processing steps only, no validation, error capturing, security issue handling, etc. included. 
 - The real project which comprises full features, UIs, history, etc. integrates several private operations (such as those of medical profession), making it impossible to be made open source.


## Guide for deploy API

Setup mysql and workbench, link here: https://dev.mysql.com/downloads/mysql/

Setup IIS, link here: https://www.iis.net/
  - Create User Bluezone and database Bluezone
  - Run sql in file ApiForApp/DB/Bluezone.sql to create structure database
  - Open ApiForApp/web.config to update appsetting connection string database MSSQL
  ```sh
  <add key="MSSQL" value="Server=localhost; Port=3306; Database=bluezone; Uid=Bluezone; Pwd=;CharSet=utf8;" /> 
  ```
  - Deploy Api on IIS


## Guide for send notification to devices (android, ios)

Setup nodejs 12.16.2, link here: https://nodejs.org/dist/v12.16.2/node-v12.16.2-x64.msi
  - Goto SendNotify folder
  - Open serviceAccountKey.json file -> Update parameters Firebase
  - At SendNotify folder open (cmd, terminal) here and execute command 'npm install' to download library
    ```sh
    $ npm install
    ```
  - Execute command 'npm start' to run port 3000
    ```sh
    $ npm start
    ```
  - Open 'localhost:3000' on browser

## Tech

Bluezone uses a number of open source projects to work properly:

* [Mysql] - Database
* [IIS] - Deploy .NET project
* [Firebase] - Database realtime
* [Bootstrap] - great UI boilerplate for modern web apps
* [node.js] - evented I/O for the backend
* [Express] - fast node.js network app framework
* [jQuery] - duh

And of course Bluezone itself is open source with a [public repository][dill]
 on GitHub.

## Licensing
Bluezone is released under GNU/GPL version 3.

See [LICENSE](LICENSE) for the full license.

## Community
  - Bluezone Fanpage: https://www.facebook.com/BluezoneVN
  - Bluezone group on FB: https://www.facebook.com/groups/BluezoneVN
  - https://groups.google.com/forum/#!forum/bluezoneglobal
