# InventoryMgtSystem-mongoDB

     frontend (Ionic): https://github.com/ninabee94/InventoryMgtSystem-Ionic4
     backend (Express.js): https://github.com/ninabee94/InventoryMgtSystem-API-Express
     database (mongoDB): https://github.com/ninabee94/InventoryMgtSystem-mongoDB
     
=======================================

<b>1. Download & install mongoDB</b>

     https://www.mongodb.com/download-center/community
     
     version: 4.0.10 (current release)
     os: windows x64 x64
     package: msi
    
<b>2. Setup mongoDB data path</b>
     
     //(open cmd admin mode)
     
     cd C:\Program Files\MongoDB\Server\4.0\bin     
     mongod.exe --dbpath "c:/program files/mongodb/server/4.0/data"
     
     //(edit security of c:/program files/mongodb/server/4.0/data to enable read & write )
     
<b>3. Create Database and table</b>

     //(open cmd admin mode)
     
     cd C:\Program Files\MongoDB\Server\4.0\bin
     mongod.exe 
     use inventory_system
     db.peoples.insert( {"email":"nabihahzahari@gmail.com", "name":"nabihah", "position":"junior", "password":"nabihah"} );
     db.items.insert( {"name":"bubble", "quantity":6, "price":1, "userid":1} );
     
     //Ctrl^C (to exit mongoDB shell)
     
<b>4. Start mongoDB service</b>

     //(open cmd admin mode)
     
     cd C:\Program Files\MongoDB\Server\4.0\bin
     mongod.exe --config "C:\Program Files\MongoDB\Server\4.0\mongod.cfg" --install
     net start MongoDB
     net stop MongoDB

<b>5. Download & install mongoDB compass</b>
     
     https://www.mongodb.com/download-center/compass
     
     hostname: localhost
     port: 20717
     
