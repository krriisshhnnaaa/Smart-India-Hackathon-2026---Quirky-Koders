# Capacity Connect — Definitions & Mathematical Formulations
Definitions
Introduction to the project

Capacity Connect is a competency-driven training ecosystem connecting trainees, trainers, courses, assessments and competency data.

The system continuously collects evidence from learning activities, assessments, trainer certifications, professional experience and learner feedback. This information is used to represent trainee progress, evaluate trainer suitability for specific courses, and provide personalized learning recommendations.

The system also provides two visual representations:

Learning Room — represents an individual trainee's learning state.
Learn-City — represents the larger trainee–trainer ecosystem.


1. Trainee

A user who enrolls in courses, attends lectures and completes assessments to develop specific competencies.

2. Trainer

A user who provides courses/lectures and possesses skills, certifications and professional experience that can be evaluated against course requirements.

3. Course

A structured learning program containing multiple topics and learning resources.

4. Topic

An individual concept or competency area within a course.

5. Competency

A measurable representation of a user's demonstrated knowledge or ability in a particular skill/topic.

6. Learning Room

A visual representation of an individual trainee's current learning state.

Courses are represented as bookshelves, topics as books, and topic-level progress as book thickness.

7. Bookshelf B(c) :
Represents course c currently being learned by the trainee.
<img width="186" height="59" alt="image" src="https://github.com/user-attachments/assets/f64dcc5c-9028-4739-8d2e-74f665218536" />

8. Book K(c,t) :
Represents topic t within course c
<img width="259" height="62" alt="image" src="https://github.com/user-attachments/assets/ffe05ac2-6fb5-41db-a27d-a65b30afeeef" />

9. Book Thickness D(c,t) :
Represents the trainee's demonstrated progress or competency in topic t of course c
<img width="259" height="62" alt="image" src="https://github.com/user-attachments/assets/1c77e75c-c8d0-45a7-8f12-e470d88f9671" />

or, 
<img width="259" height="62" alt="image" src="https://github.com/user-attachments/assets/a3cc8382-d1d3-4508-8724-f5f2b4f4f4fd" />

where \(0\) represents no demonstrated progress and 1/100 represents complete competency.

10. Learn-City

A 2D visual representation of the platform's learning ecosystem.

Each subject has corresponding trainee and trainer sectors. The sectors share a colour identity while using different building types to distinguish trainees from trainers

11. Sector

A region of Learn-City representing a particular subject.

Each subject has:
<img width="476" height="136" alt="image" src="https://github.com/user-attachments/assets/775830eb-f97e-4db1-b354-b53d5c925c32" />
12. Sector Colour

The visual identity assigned to a subject.

The same subject uses the same colour family in both its trainee and trainer sectors.
For example:
<img width="476" height="136" alt="image" src="https://github.com/user-attachments/assets/6c34f578-3a7b-4012-92c2-2a81e79a569b" />

while their building types remain different.

13. Trainee Building

A building representing a group of trainees studying the same subject.

If each building has a maximum capacity of C(B), the number of buildings required is:
<img width="261" height="137" alt="image" src="https://github.com/user-attachments/assets/8cd9c8bf-6f37-4ea3-ab77-77b873665437" />
where, 
<img width="714" height="186" alt="image" src="https://github.com/user-attachments/assets/b5159d4c-a1db-43d5-9116-4b19706dce3f" />
For the proposed implementation:
<img width="228" height="147" alt="image" src="https://github.com/user-attachments/assets/e06f8d1d-9939-4964-9269-7628252a0a47" />

therefore:
14. Trainer Building

A building representing one trainer within a trainer sector.

<img width="470" height="68" alt="image" src="https://github.com/user-attachments/assets/e90dd5c6-43ed-4f81-8eb0-5e2303b35915" />

Therefore, for m trainers:
<img width="470" height="68" alt="image" src="https://github.com/user-attachments/assets/01056818-7e02-4e44-ae36-eebecd17428e" />

The size of the trainer building is determined by the trainer's suitability for the corresponding course/subject.

15. Trainer Suitability

A course-specific measurement of how suitable a trainer is for teaching a particular course.
<img width="182" height="73" alt="image" src="https://github.com/user-attachments/assets/ca43bcc5-bc68-4180-99a0-c203b0bca7cc" />

represents the suitability of a trainer for course \(c\).

The same trainer can therefore have different suitability values for different courses:
<img width="517" height="98" alt="image" src="https://github.com/user-attachments/assets/dc78f8c3-ec1c-4ae9-9e56-1e2582c6e448" />

