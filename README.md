# HPCC
Configuration files for HPCC for Mac OSX

Make sure /opt/HPCCSystems/bin is in your path.
Clone this repository.
Replace /var/lib/HPCCSystems with the content of var_lib_hpccsystems.zip
```
sudo rm -fr /var/lib/HPCCSystems
sudo unzip var_lib_hpccsystems.zip -d /var/lib
chmod -R a+rwx /var/lib/HPCCSystems
```

Then, from the directory containing the xml files in this repository, you can run:
* **daserver** (Runs the Dali server, which is the persistence mechanism for HPCC)
* **esp** (Runs the ESP server, which is the web services and UI layer for HPCC)
* **eclccserver** (Runs the ECL compile server, which takes the ECL and compiles it down to C and then a dynmic library)
* **roxie** (Runs the Roxie server, which is capable of responding to queries)

If you kickoff each one of those, then you should be ready to run some ECL. 
Go to http://localhost:8010 in a browser.
