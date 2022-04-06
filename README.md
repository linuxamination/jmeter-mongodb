## LinuXamination 

### JMeter Mongodb Test Plan

To export the database test in the mongodb :
1) Unzip dump.zip
2) cd into the parent directory of dump folder. Do not 'cd' into the dump folder.
3) Run command
sudo mongorestore
4) It will create a db test and a collection zips with data in the test.

To run the test Plan in the JMeter :
a) Once database is imported, open the mongodb.jmx file in the JMeter.
b) Put your mongodb parameters in user defined variables section of Test Plan.
c) Run the test plan. Make sure request 'connect' is always enabled.

i) If you want to fetch the data using csv, update the csv path, where your csv file is present, in the csv dataset config.
ii) Enable the Loop Controller.
iii) To fetch all the records of csv, Make sure Loop count of Loop Controller should be same as the number of entries in the csv file.
iv) Run the test plan.

