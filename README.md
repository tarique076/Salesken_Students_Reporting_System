<h1>Student Reporting System</h1>

This application was built as an assignment for Salesken recruitment process. It is a student reporting system where we can add students, get percentage of marks of whole class, get average marks of students and get top two performing students.

### Tech-Stacks Used
- Spring Boot
- Spring Framework
- Spring Data JPA
- Java
- Layered Architechture
- Lombok
- ElasticSearch
- Kibana

## Installation & Run 
ElasticSearch required to be installed to run the application.
````
  Install ElasticSearch.
  Change Configuration. (ElasticSearch\config\elasticsearch.yaml).
  Edit the above file. Comment all security related configs.
  Add the below code to this file.

  ingest.geoip.downloader.enabled: false
  xpack.security.enabled: false
  xpack.security.transport.ssl.enabled: false
  xpack.security.http.ssl.enabled: false

  Change cluste.name to student_reporting_system
  Change path.data to the path where application is present.

````

<h2>Api Endpoints</h2>

* http://localhost:8090/home       (HomePage)
* http://localhost:8090/addStudent  (Add a Student)
* http://localhost:8090/getClassPercentage    (Get percentage marks of whole class)
* http://localhost:8090/subjectAvg   (Check average marks of a subject)
* http://localhost:8090/topTwoStudents   (Check top two students.)
* http://localhost:8090/getAllStudents    (Check all students details)

