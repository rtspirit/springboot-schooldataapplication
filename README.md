# springboot-schooldataapplication
A School Data Spring Boot Application consisting of three entities: Topics, Courses, Lessons.<br>
Integrated with Apache Derby Runtime Database.<br>

## Routes:<br>
### Topics:<br>

**GET** : `/topics`<br>
**GET** : `/topics/{id}`<br>
**POST** : `/topics`<br>
**PUT** : `/topics/{id}`<br>
**DELETE** : `/topics/{id}`<br>

### Courses:<br>

**GET** : `/topics/{id}/courses`<br>
**GET** : `/topics/{topicId}/courses/{id}`<br>
**POST** : `/topics/{topicId}/courses`<br>
**PUT** : `/topics/{topicId}/courses/{id}`<br>
**DELETE** : `/topics/{topicId}/courses/{id}`<br>

### Lessons:<br>

**GET** : `/topics/{topicId}/courses/{id}/lessons`<br>
**GET** : `/topics/{topicId}/courses/{courseId}/lessons/{id}`<br>
**POST** : `/topics/{topicId}/courses/{courseId}/lessons`<br>
**PUT** : `/topics/{topicId}/courses/{courseId}/lessons/{id}`<br>
**DELETE** : `/topics/{topicId}/courses/{courseId}/lessons/{id}`<br>

### Following relationships are used for database entities:<br>
*Topics can have many Courses*<br>
*Courses can have many Lessons*<br>
