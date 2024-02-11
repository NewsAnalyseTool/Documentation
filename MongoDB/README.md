# Documentation of MongoDB

You have to update the following lines 8, 17, 33. You have to use your system path.\
Line 8 for data storage. Line 17 for logging and Line 33 for Security keyfile.\

# Linux
These .conf files have to be in "/etc/".\
You have to enable MongoDB by using systemctl.
- systemctl enable mongod.conf
- systemctl enable mongod_repl1.conf
- systemctl enable mongod_repl2.conf

And start MongoDB.
- systemctl start mongod.conf
- systemctl start mongod_repl1.conf
- systemctl start mongod_repl2.conf

# MongoDB Databases and Collections
Database (Collections) you have to create
- BBC (BBC_raw_data, bbcAnalysis)
- Reddit (reddit_raw_data, redditAnalysis)
- Tagesschau (tagesschau_raw_data, tagesschauAnalysis)

# Security
You have to generate a keyfile for Security concerns between the MongoDB replica set [How to create a keyfile](https://www.mongodb.com/docs/manual/tutorial/deploy-replica-set-with-keyfile-access-control/).\
Line 32 "authorization: enabled" see [SCRAM authentication](https://www.mongodb.com/docs/manual/tutorial/configure-scram-client-authentication/)\