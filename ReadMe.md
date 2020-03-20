# Task 3 - Multi Vagrant Machine


### In order to use this VM:
`git clone git@github.com:victorsibanda/VagrantTask23.git`


### To Run Use:

`vagrant up`


#### For app

`vagrant ssh app`
`sudo node app.js`

Go to  ---> https://development.local:3000/

#### For db

`vagrant ssh db`

###### To Edit the Mongo DB Conf file Use:

```bash

sudo nano /etc/mongod.conf

#Change bind IP to 0.0.0.0
#ctrl O - To Save, Enter File Name and Press Enter
#ctrl X - To exit

exit #To leave vagrant ssh

vagrant reload #This restarts mongo services changing the config file
```


#### To test everything  

Use terminal from `vagranttask23` to navigate to:
- `cd test`
- `cd spec`
- Then `rake spec` - to run the tests. 
