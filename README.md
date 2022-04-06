## LinuXamination 

### JMeter Mongodb Test Plan

To export the database test in the mongodb :
1) Unzip dump.zip
2) cd into the parent directory of dump folder. Do not 'cd' into the dump folder.
3) Run command
sudo mongorestore
4) It will create a db test and a collection zips with data in the test.

To run the test Plan in the JMeter :
1) Once database is imported, open the mongodb.jmx file in the JMeter.
2) Put your mongodb parameters in user defined variables section of Test Plan.
3) Run the test plan. Make sure request 'connect' is always enabled.

1) If you want to fetch the data using csv, update the csv path, where your csv file is present, in the csv dataset config.
2) Enable the Loop Controller.
3) To fetch all the records of csv, Make sure Loop count of Loop Controller should be same as the number of entries in the csv file.
4) Run the test plan.

