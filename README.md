Installation 
  npm install -g newman
  npm install newman newman-reporter-htmlextra

To run Collection 
   newman run Restful-Booker.postman_collection.json -e "Test Environment.json" -r htmlextra --reporter-htmlextra-export "reports/Execution_report.html"
  
