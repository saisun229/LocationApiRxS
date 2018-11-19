# LocationApiRxS


PREREQUISITES:

1.Spring Tool Suite
2.Mysql Workbench

STEPS:

Step 1: Extract Zip folder
Step 2: Open Mysql Workbench
Step 3: Create a schema with name pharmacyloc
Step 4: Open the extracted folder (Application) in Spring Tool Suite.
step 5: Open the file under LocationApiRxS/src/main/resources/application.properties 
step 5: Make sure these properties hold right values
		 
         spring.datasource.url = jdbc:mysql://localhost:3306/pharmacyloc       (schema name from step 2)
         spring.datasource.username = root                                     (Yours mysql workbench username Ex:root)
         spring.datasource.password = root                                     (Yours mysql workbench password Ex:root)
	
step 6: Run spring boot application in Spring Tool Suite
step 7: Open Postman Application.
step 8: Use POST and Enter latitude and longitude values in to the URL
        Example:       http://localhost:8085/location?latitude=39.05167&longitude=-95.78524
step 9: You will get the response :) Thanks
          
SAMPLE RESPONSE PACKET:
		
	[
    {
        "id": 16,
        "name": "TALLGRASS PHARMACY",
        "address": "601 SW CORPORATE VIEW",
        "city": "TOPEKA",
        "state": "KS",
        "zip": 66615,
        "latitude": 39.05716,
        "longitude": -95.76692
    },
    1.6956018227576095
    ]

Nearest pharmacy from user & Distance in miles: 1.6956018227576095
