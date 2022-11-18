# springboot-schooldataapplication
A School Data Spring Boot Application consisting of three entities: Topics, Courses, Lessons.<br>
Integrated with Apache Derby Runtime Database.<br>

## Routes:<br>
### Topics:<br>

**GET** : > /topics
**GET** : > /topics/{id}
**POST** : > /topics
**PUT** : > /topics/{id}
**DELETE** : > /topics/{id}

### Courses:<br>

**GET** : > /topics/{id}/courses
**GET** : > /topics/{topicId}/courses/{id}
**POST** : > /topics/{topicId}/courses
**PUT** :  > /topics/{topicId}/courses/{id}
**DELETE** : > /topics/{topicId}/courses/{id}

### Lessons:<br>

**GET** : > /topics/{topicId}/courses/{id}/lessons
**GET** : > /topics/{topicId}/courses/{courseId}/lessons/{id}
**POST** : > /topics/{topicId}/courses/{courseId}/lessons
**PUT** : > /topics/{topicId}/courses/{courseId}/lessons/{id}
**DELETE** : > /topics/{topicId}/courses/{courseId}/lessons/{id}

### Following relationships are used for database entities:<br>
*Topics can have many Courses*<br>
*Courses can have many Lessons*<br>
