---
title: Syllabus
navbar: Syllabus
tas:
  - name: 'Eve Matson'
    foto: '/images/matson.jpeg'

  - name: 'Jose Corella'
    foto: '/images/corella.jpg'

  - name: 'Xiaochen (Chris) Li'
    foto: '/images/li.jpg'

cutoff1: 2020-04-03
cutoff2: 2020-05-07

---

<style>
.notification {
  padding: .75rem !important;
  font-size: 0.75rem;
}
</style>

This syllabus is similar to a contract between students and the instructor, and as such it is quite long (with many sections required by the university). A few key points from this syllabus are highlighted here:

  - Use Piazza for all course communication. See: [Communication Policy](#communication-policy).

  - You should be stuck for 30 minutes on a problem before seeking help, but you should definitely seek help if you have been stuck for over an hour. See: [Getting Help](#getting-help).

  - Do not cheat. This includes working too closely with your classmates, teacher assistants, CS tutors, or past students. See: [Cheating Policy](#cheating-policy).

  - You must pass at least one exam to avoid an automatic F in this class. See: [Pass Requirements](#pass-requirements).

  - You must pass enough projects before the withdraw deadline to avoid an automatic F in this class. See: [Pass Requirements](#pass-requirements).

  - Treat this class like a part-time job and plan to spend 10 to 20 hours coding per week outside of class. See: [Credit Hour Policy](#credit-hour-policy).

Students are still required to read through the entire syllabus below.

### CS 212 Software Development
{: .title }

#### Spring 2020 &bull; 4 Credits
{: .subtitle .has-text-weight-light }

{{ site.data.info.blurb }}

[CS 212 Course Catalog](https://www.usfca.edu/catalog/course/212-software-development){: .button .is-link}

### Lecture Sections

The class times for {{ site.data.info.code }} are:

<div class="columns">
  <div class="column is-narrow">
    <strong>CS 212-01 (CRN 20962)</strong><br/>
    <i class="fa-fw fas fa-calendar-alt"></i>
    Tuesdays, Thursdays<br/>
    <i class="fa-fw fas fa-clock"></i>
    12:45pm &ndash; 2:30pm<br/>
    <i class="fa-fw fas fa-map-marker-alt"></i>
    <a href="https://www.usfca.edu/campus-buildings-services/main-campus/cowell">Cowell Hall 214</a>
  </div>
</div>

Class time will consist of traditional lectures, live coding sessions, quizzes, discussions, guest speakers, and more. Most lectures will be recorded and live-streamed via [Zoom]({{ site.data.info.links.stream.link }}).

### Lab Sessions

Students should plan to attend one lab session per week. The lab sessions are:

<div class="columns">
  <div class="column is-narrow">
    <strong>CS 212L-01 (CRN 22154)</strong><br/>
    <i class="fa-fw fas fa-calendar-alt"></i>
    Fridays<br/>
    <i class="fa-fw fas fa-clock"></i>
    2:15pm &ndash; 3:20pm<br/>
    <i class="fa-fw fas fa-map-marker-alt"></i>
    <a href="https://www.usfca.edu/campus-buildings-services/main-campus/lo-schiavo">Lo Schiavo Science G12</a>
  </div>
</div>

Lab sessions give students an additional opportunity to interact with teacher assistants and meet with the instructor for one-on-one code reviews.

### Instructor

The course instructor and office hours will be as follows:

<div class="columns">
  <div class="column is-narrow">
    <div class="box">
      <!-- nested columns for profile photo -->
      <div class="columns is-mobile is-variable is-1">
        <div class="column is-narrow">
          <div class="image is-64x64">
            <img class="is-rounded" src="/images/engle.png">
          </div>
        </div>

        <div class="column">
          <strong>Sophie Engle</strong><br/>
          <i class="fa-fw fas fa-calendar-alt "></i>
          <span>Mondays, Thursdays</span>
          <br/>

          <i class="fa-fw fas fa-clock "></i>
          <span>2:45pm &ndash; 4:15pm</span>
          <br/>

          <i class="fa-fw fas fa-map-marker-alt "></i>
          <a href="https://www.usfca.edu/campus-buildings-services/main-campus/harney-science">Harney Science 412B</a>
          <br/>

          <i class="fa-fw fas fa-globe "></i>
          <a href="//sjengle.cs.usfca.edu">sjengle.cs.usfca.edu</a>
        </div>
      </div>
      <!-- end nested columns -->
    </div>
  </div>
</div>

<i class="fas fa-envelope-open-text"></i>
See the [Communication Policy](#communication-policy) for how to contact the instructor and teacher assistants.
{: .notification }

### Teacher Assistant(s)

The teacher assistant(s) assigned to this course are:

<div class="columns">
  {% for ta in page.tas %}
  <div class="column is-narrow">
    <div class="box">
      <!-- nested columns for profile photo -->
      <div class="columns is-mobile is-variable is-1">
        {% if ta.foto %}
        <div class="column is-narrow">
          <div class="image is-64x64">
            <img class="is-rounded" src="{{ ta.foto | relative_url }}">
          </div>
        </div>
        {% endif %}

        <div class="column">
          <strong>{{ ta.name }}</strong><br/>
          <i class="fa-fw fas fa-map-marker-alt "></i>
          <a href="https://www.usfca.edu/campus-buildings-services/main-campus/harney-science">Harney Science 411</a>
        </div>
      </div> <!-- end nested columns -->
    </div>
  </div>
  {% endfor %}
</div>

Teacher assistant responsibilities and office hours will be posted on [Piazza]({{ site.data.info.links.piazza.link }}) at the start of the semester.

<i class="fas fa-envelope-open-text"></i>
See the [Communication Policy](#communication-policy) for how to contact the instructor and teacher assistants.
{: .notification }

### Prerequisites

Students must have completed [CS 112 Introduction to Computer Science II](https://www.usfca.edu/catalog/course/112-introduction-computer-science-ii) and [CS 245 Data Structures and Algorithms](https://www.usfca.edu/catalog/course/245-data-struct-algorithms) with grades of C or better before taking this class.

### Learning Outcomes

At the end of this course, students should be able to:

- Independently design programs
- Produce professional-quality source code
- Implement large programs with 1,000 to 2,000 source lines of code (SLOC)
- Design and execute tests to find and repair software bugs
- Redesign and refactor code to improve quality

Assessment of these outcomes will be done by a combination of quizzes, exams, homework, projects, and code review. See [Course Requirements](#course-requirements) below for details.

### Required Materials

There are no required materials for this class.

If students do not have access to their own laptop or computer, they may utilize one of the CS lab computers for completing assignments.

### Important Dates

The following are important dates and deadlines for the course. These dates are fixed (i.e. they should not change as the semester progresses).

<style>
table.dates tr td:nth-child(2) {
  white-space: nowrap;
}

table.dates tr:nth-child(1),
table.dates tr:nth-child(2),
table.dates tr:nth-child(3),
table.dates tr:nth-child(4),
table.dates tr:nth-child(6),
table.dates tr:nth-child(8),
table.dates tr:nth-child(9),
table.dates tr:nth-child(12) {
  color: grey;
}
</style>

| Week   | Date  | Description |
|:------:|------:|:------------|
| 01     | 01/21 | **Lectures Begin:** First day of class. |
| 02     | 01/27 | **Add Deadline**: Last day to add classes. |
| 03     | 02/07 | **Drop Deadline**: Last day to drop with a 100% refund. Courses/sections dropped after this date appear with a neutral "W" on transcript. |
| 05     | 02/17 | **President's Day**: No classes or office hours will be offered this day. |
| 07     | 03/03 | **Exam 1**: First exam, followed by retake opportunity on Thursday. |
| 08     | 03/09--03/13 | **Spring Break**: No classes or office hours will be offered this week. |
| 11     | {{ page.cutoff1 | date: "%m/%d" }} | **Project Cutoff 1**: Last day to satisfy project pass requirement 1 to avoid an automatic F letter grade. |
| 12     | 04/06 | **Withdraw Deadline**: Last day to withdraw from classes with a neutral "W" on transcript. |
|        | 04/10 | **Easter Holiday**: No labs, code reviews, or office hours will be offered this day. |
| 15     | 04/28 | **Exam 2**: Second exam, followed by retake opportunity on Thursday. |
| 16     | {{ page.cutoff2 | date: "%m/%d" }} | **Project Cutoff 2**: Last day to satisfy project pass requirement 2 to avoid an automatic F letter grade. |
|        | 05/07 | **Lectures End**: Last day of class. |
| Finals | 05/09--05/14 | **Final Code Reviews**: Last project code review. |
{: class="table dates is-hoverable" style="width: auto;"}

Instead of a final exam, there will final project code reviews during finals week.

See the [Schedule]({{ "/schedule.html" | relative_url }}) for the latest weekly schedule. See the [Academic Calendar](https://myusf.usfca.edu/registration/academic-calendar) for university-wide important dates.


------

## Course Requirements
{: .is-uppercase }

This section covers how the learning outcomes for this course will be assessed. This course will be a hybrid flipped classroom, with an emphasis on mastery learning. The majority of the grade will be derived from projects and exams. See the following subsections for details.

### Pass Requirements

To ensure students are meeting the [learning outcomes](#learning-outcomes) for this course, students must meet the following minimum requirements to receive a non-failing grade (D- or higher) in this course:

  - **Exam Pass Requirement:** Students must receive a C letter grade or higher on at least one exam (including retakes).

  - **Project Pass Requirement 1:** Students must pass project 1 tests, project 1 code review, and project 2 tests by the project cutoff 1 deadline on {{ page.cutoff1 | date: "%A %B %d, %Y" }}.

  - **Project Pass Requirement 2:** Students must pass project 2 code review and project 3 tests by the project cutoff 2 deadline on {{ page.cutoff2 | date: "%A %B %d, %Y" }}.

**Failure to meet 1 or more of the following requirements will result in an automatic F letter grade for this course, regardless of what your current letter grade is in Canvas.**
{:.has-text-danger}

If students are concerned about not meeting one or more of these requirements by the withdraw deadline, they are encouraged to withdraw from the class to avoid the F letter grade on their transcripts. Note, however, that a W (withdraw) counts as an attempt and CS majors and minors have restrictions on how many times they may attempt CS courses.

Meeting the pass requirements does not guarantee a passing grade. See the [Grade Breakdown](#grade-breakdown) section below for how the final grade will be calculated.

### Grade Breakdown

If the [pass requirements](#pass-requirements) are met, then the final letter grade for this class will be calculated as follows:

| Percent | Category        |
|--------:|:----------------|
|      5% | Participation   |
|      5% | Quizzes         |
|     10% | Homework        |
|     20% | Exams           |
|     60% | Projects        |
{: class="table is-hoverable" style="width: auto;"}

The assignments within each category are not necessarily equally weighted. For example, some participation assignments are worth more points than others.

Each of these categories are described more below.

#### Participation

Participation includes pass/fail assignments such as participating in surveys, discussions on Piazza, in-class exercises, attending labs, lab exercises, and participating in other on-campus or off-campus CS events.

*Late submissions are not accepted for participation assignments.*{:.has-text-danger} However, the lowest participation grade will be dropped at the end of the semester.

#### Quizzes

Quizzes are sometimes given unannounced at the start of class, but students will often be given an opportunity to retake those quizzes. Quizzes will be conducted on [Canvas]({{ site.data.info.links.canvas.link }}), and the answers will automatically be released after the quiz deadline.

*Late submissions are not accepted for quizzes.*{:.has-text-danger} However, the lowest quiz grade will be dropped at the end of the semester.

#### Homework

Homework programming assignments are assigned on a semi-weekly basis, and usually due the following week. Students may work on these assignments during their lab session, allowing them to get immediate help from the teacher assistants.

Partial grades are not given for homework assignments; students must pass 100% of the provided tests to earn credit. If all of those tests pass before the deadline, the student will earn a 100% on that homework assignment.

Otherwise, there will be a --5% deduction per day (24 hours) the homework is late based on the commit timestamp of the repository. Homework will not be accepted if it is more than one week late.

The lowest homework assignment grade will be dropped at the end of the semester.

#### Exams

There will be two exams. The exams are *not* comprehensive. Each exam will have a retake opportunity where students may earn back a small fraction of the points missed on the original attempt. See [Important Dates](#important-dates) for the exact exam and exam retake dates.

Instead of a final exam, students will have a final project graded during finals week. A signup sheet will be posted towards the end of the semester. If you have travel plans during finals week, please confirm your travel dates first with the instructor.

Students must receive a C letter grade or higher on at least one exam (including retakes). See the [Pass Requirements](#pass-requirements) for more.

#### Projects

Programming projects place an emphasis on code quality&mdash;it is not enough to achieve correct results. Each project must pass several functionality tests and then undergo multiple rigorous code reviews checking for specific criteria, such as proper encapsulation and generalization, efficiency, and maintainability.

We use a **mastery learning** approach with projects: students must perfect the current project before moving on to the next project. The final project grade will depend on when and how many projects are completed.

Each project grade is split into two components: functionality (evaluated with automated software tests) and design (evaluated with one-on-one code reviews). The project functionality must be passed before the code review may be passed, students must pass code review for each project sequentially, and may only have one review appointment per week.

The functionality grade depends on when the project passes the tests. Projects that pass the functionality tests by the checkpoint will receive a 100%. Otherwise, there will be a --10% deduction for each week the project is late past the checkpoint up to a maximum --30% deduction. The code review grade will be 100% once passed, minus any deductions due to submission issues. For example, failing to fix all of the issues from a previous code review may result in a --5% to --10% deduction.

There are only 2 hard deadlines for projects: the project cutoff 1 deadline on {{ page.cutoff1 | date: "%A %B %d, %Y" }} before the withdraw deadline, and the project cutoff 2 deadline on {{ page.cutoff2 | date: "%A %B %d, %Y" }} at the end of the semester. If a cutoff deadline is missed, all incomplete project grades default to 0%. See the [Pass Requirements](#{{ "Pass Requirements" | slugify }}) for details.

### Grading Scale

The following is the grading scale mapping percentage to letter grade and GPA for this course:

<style>
table.gpa tbody tr:nth-child(n+9) {
  background-color: #CD542C;
  color: white;
}
</style>

|          | Letter |        | GPA |
|---------:|:-------|:-------|:---:|
| 97% &le; | A+     | < 100% | 4.0 |
| 94% &le; | A      | < 97%  | 4.0 |
| 90% &le; | A--    | < 94%  | 3.7 |
| 87% &le; | B+     | < 90%  | 3.3 |
| 84% &le; | B      | < 87%  | 3.0 |
| 80% &le; | B--    | < 84%  | 2.7 |
| 77% &le; | C+     | < 70%  | 2.3 |
| 74% &le; | C      | < 77%  | 2.0 |
| 70% &le; | C--    | < 74%  | 1.7 |
| 67% &le; | D+     | < 70%  | 1.3 |
| 64% &le; | D      | < 67%  | 1.0 |
| 60% &le; | D--    | < 64%  | 0.7 |
|  0% &le; | F      | < 60%  | 0.0 |
{: class="table gpa" style="width: auto;"}

Non-passing grades for undergraduate students are highlighted in <span class="tag is-danger">red</span>. See the [Undergraduate Student Regulations](https://catalog.usfca.edu/content.php?catoid=4&navoid=225#grading-system) for more about letter grades and GPA for undergraduate students.

### Student Awards

At the end of the semester, various awards will be given to students. While these awards are informal and do not impact your final grade, they do provide a way for students to differentiate themselves on resumes. Example awards include: top student askers and answerers on Piazza, and more.

------

## Course Policies
{: .is-uppercase }

This section includes miscellaneous policies specific to this course, including communication, attendance, credit hours, cheating, and more. These policies are in addition to the standard USF policies included later.

### Communication Policy

Most course-related communication will be handled using [Piazza]({{ site.data.info.links.piazza.link }})---a FERPA-compliant Q&A platform that supports public, anonymous, and private posts. When making posts on Piazza, please keep the following in mind:

  - **Make a public post when appropriate.** This lets us answer questions once for all students. You can **post anonymously** if you are uncomfortable with attaching your name to a post or a response. When posting anonymously, your classmates will not be able to see your identity but instructors will still be able to see your name. This is necessary to give you credit for participation and ensure everyone is following the code of conduct.

      *If you send an email to the instructor or teacher assistant, or make a private post that should be public, you will be asked to create a new public anonymous post on Piazza before receiving an answer.*

  - **Do not post code on Piazza.** If you have a question regarding your specific code, please commit and push your code to your GitHub repository and [post a link](https://help.github.com/en/articles/creating-a-permanent-link-to-a-code-snippet) directly to the relevant code. That ensures only those with access to your repository (instructor and teacher assistants) will see your code.

  - Make posts regarding grades or specific solutions private to the instructor and teacher assistants. When making private posts, they should always be marked as visible by both the instructor and teacher assistants so there is no confusion.

In addition to [Piazza]({{ site.data.info.links.piazza.link }}), the instructor will also use [Canvas]({{ site.data.info.links.canvas.link }}) to notify students of missing assignments or warn about low grades. Both the instructor and teacher assistants will use [Github]({{ site.data.info.links.github.link }}) for project-related communication. You may also ask for help in-person during office hours or lectures. These are the only officially approved channels of communication for contacting the instructor or teacher assistants.

**Under no circumstances should you reach out to the teacher assistants via any unapproved communication channel.**{: .has-text-danger }
Instructors and teacher assistants must provide all students equal opportunity for course-related help. Using unapproved communication channels creates an unfair advantage over other students and will be treated as a violation of the [Student Conduct Code](https://myusf.usfca.edu/fogcutter).

<i class="fas fa-sms"></i>
For example, it is appropriate to use text messages to invite a teacher assistant to lunch as friends. It is NOT appropriate to start asking that teacher assistant questions about the course during that lunch! It is also NOT appropriate to directly text message course-related questions to that teacher assistant, even if you are friends and were able to get help from them before. You can, however, ask that teacher assistant for help during official office hours.
{: .notification }

### Getting Help

Stuck? A good rule of thumb is to struggle with solving a problem for at least 30 minutes before asking for help. However, if you are still stuck after 1 hour, seek help. There are many ways to get help with this class:

  - Ask questions on [Piazza]({{ site.data.info.links.piazza.link }}). Most questions receive a response in under 24 hours (sometimes within 30 minutes). You may figure out your problem before you get a response, but then you can delete your question or mark it as solved.

  - Ask questions during the instructor office hours. Office hours are first-come first-serve and there is lots of seating (including power outlets for charging).

  - Ask the teacher assistants for help during lab sessions or their office hours. All of the teacher assistants for this course took CS 212 previously with Professor Engle.

  - Ask a tutor for help at the [CS Tutoring Center](http://tutoringcenter.cs.usfca.edu/). Many of the tutors took CS 212 previously (and many of them also took it with Professor Engle). However, even tutors that did not take CS 212 may be able to help. Sometimes, it just helps to talk about your code with someone (see [rubber duck debugging](https://en.wikipedia.org/wiki/Rubber_duck_debugging)).

  - Ask your classmates for high-level help or hints, but be careful! To avoid violating the cheating policy and honor code, make sure you never share code with your classmates or look at the code of your classmates.

If you are feeling generally overwhelmed (including emotionally) and need advice, do not hesitate to reach out to the instructor. Since office hours can be crowded at times, you are welcome to schedule an appointment with the instructor via Piazza to chat in private.

<i class="fas fa-award"></i>
Awards are given out at the end of the semester to students with the top questions and answers on Piazza. This is one way to distinguish yourself from others on your resume!
{: .notification }

### Attendance Policy

Students are expected to be on-time to all classes to minimize disruption. Attendance is mandatory for all exams, guest speakers, and in-class exercises. These dates will be posted on the course schedule. Attendance must be in person; joining the livestream does *not* count.

Attendance is mandatory for all one-on-one code review appointments. Students must be on-time to these appointments. If a student arrives more than 5 minutes late, the appointment will be canceled. *Students risk a grade penalty for repeated canceled or missed appointments.*{:.has-text-danger}

### Credit Hour Policy

All courses must comply with the [Credit Hour Policy](https://myusf.usfca.edu/sites/default/files/usf_credit_hour_policy_0.pdf), which states:

  > "One unit of credit in lecture, seminar, and discussion work should approximate one hour of direct faculty instruction and a minimum of two hours of out-of-class student work per week through one 15-week semester."

As this is a 4 credit course, students must spend a **minimum** of 8 hours of out-of-class work per week to earn a non-failing (D&ndash; or higher) letter grade. To earn a passing C or higher letter grade (as required for the CS major), students should expect to spend closer to **10 to 20 hours per week** on projects, homework, and participation assignments.

Think of this class like a part-time job. If you do not put in the time, you will not make it to the final project. Many students do not pass due to poor time management!
{: .notification }

### Cheating Policy

All students are expected to know and adhere to the University's [Honor Code](https://myusf.usfca.edu/academic-integrity/). In short, students must never represent another person's work as their own. Examples of honor code violations include (but are not limited to):

  - Copying and pasting code (especially without attribution) from the web

  - Having anyone other than yourself complete your work (including teacher assistants, tutors, and former students)

  - Working too closely with others such that your code no longer represents an individual contribution

  - Sharing your solutions with others (either directly or indirectly)

Keep in mind that unauthorized collaboration or discussion that results in the same or very similar work indicates that you have not placed enough independent thought into your submission and is a violation of the honor code, regardless of whether you directly copied!

**Flagrant or repeat violations of the honor code will result in an F in the course, a report to the Academic Integrity Committee (AIC), and a report to the Dean.**{: .has-text-danger }
At the discretion of the instructor, a less severe penalty may be imposed for minor or first offenses. This is at the sole discretion of the instructor and any violation may result in an F in the course.

<i class="fas fa-exclamation-triangle"></i>
Keep in mind that there is a history of your code development on Github. **Commit and push changes often** to record your incremental code development.
{: .notification }

### Extra Credit Policy

Student may request **one extra credit/makeup opportunity** for assignments in the participation, homework, or project categories. Students may earn up to 50% of the amount of points missed on that assignment. For example, suppose if a student earned 70 out of 100 points on an assignment, that student can request an extra credit opportunity to make up 15 points. Requests must be made on Piazza. Students may make only one request; choose wisely to maximize the impact on the final grade.

Extra credit requests may not be made for quizzes or exams.

### Policy Exceptions

Exceptions to most course policies are made only in the case of **verifiable exceptional circumstances**. This includes medical emergencies, mental health and well-being crises, or family-related emergencies. Extensions must be arranged prior to the original deadline unless in case of extreme emergency (such as an emergency room visit).

If you need to miss class for a family event (such as a wedding or graduation) or academic/professional conference (such as Grace Hopper or an internship interview), contact the instructor ahead of time to make arrangements. Keep in mind you will likely be asked to submit assignments *early* versus getting an extension. Please note exceptions will not be made for other events (such as concerts, comic cons, and so on).

------

## University Policies
{: .is-uppercase }

This section includes standard statements on University policies and resources, including: disclaimers on confidentiality, mandatory reporting, sexual assault; statements regarding USF's Honor Code and Academic Integrity and behavioral expectations; important campus resources for student health, safety, and wellbeing.

### Students with Disabilities

If you are a student with a disability or disabling condition, or if you think you may have a disability, please contact [USF Student Disability Services (SDS)](https://myusf.usfca.edu/sds) for information about accommodations.

### Behavioral Expectations

All students are expected to behave in accordance with the [Student Conduct Code](https://myusf.usfca.edu/fogcutter) and other University policies.

### Academic Integrity

USF upholds the standards of honesty and integrity from all members of the academic community. All students are expected to know and adhere to the University's [Honor Code](https://myusf.usfca.edu/academic-integrity/).

### Communication

All course communications, like all other USF communications, will be sent to your USF official email address. You are therefore strongly encouraged to monitor that email account.

### Counseling and Psychological Services (CAPS)

CAPS provides confidential, free [counseling](https://myusf.usfca.edu/student-health-safety/caps) to student members of our community.

### Confidentiality, Mandatory Reporting, and Sexual Assault

For information and resources regarding sexual misconduct or assault visit the [Title IX](https://myusf.usfca.edu/TITLE-IX) coordinator or USF's [Callisto website](http://usfca.callistocampus.org/).


{% comment %}

<hr>

{% include anchor.html level="h2" text="Course Requirements" class="is-uppercase" %}

This section covers how the learning outcomes for this course will be assessed. This course will be a hybrid flipped classroom, with an emphasis on mastery learning. The majority of the grade will be derived from projects and exams. See the following subsections for details.

{% include anchor.html level="h3" text="Pass Requirements" %}

To ensure students are meeting the [learning outcomes](#{{ "Learning Outcomes" | slugify }}) for this course, students must meet the following minimum requirements to receive a non-failing grade (D- or higher) in this course:

  - **Exam Pass Requirement:** Students must receive a C letter grade or higher on at least one exam (including retakes).

  - **Project Pass Requirement 1:** Students must pass project 1 tests, project 1 code review, and project 2 tests by the project cutoff 1 deadline.

  - **Project Pass Requirement 2:** Students must pass project 2 code review and project 3 tests by the project cutoff 2 deadline.

**Failure to meet 1 or more of the following requirements will result in an automatic F letter grade for this course, regardless of what your current letter grade is in Canvas.**
{:.has-text-danger}

If students are concerned about not meeting one or more of these requirements by the withdraw deadline, they are encouraged to withdraw from the class to avoid the F letter grade on their transcripts. Note, however, that a W (withdraw) counts as an attempt and CS majors and minors have restrictions on how many times they may attempt CS courses.

Meeting the pass requirements does not guarantee a passing grade. See the [Grade Breakdown](#{{ "Grade Breakdown" | slugify }}) section below for how the final grade will be calculated.

{% include anchor.html level="h3" text="Grade Breakdown" %}

If the [pass requirements](#{{ "Pass Requirements" | slugify }}) are met, then the final grade will be calculated as follows:

<table class="table is-hoverable" style="width: auto;">
  <thead>
    <tr>
      <th>Category</th>
      <th>Percent</th>
    </tr>
  </thead>

  <tbody>
    {% for element in site.data.syllabus.grade_breakdown %}
    <tr>
      <td>
        <a href="{{ element.link }}">
          {{ element.text }}
        </a>
      </td>

      <td class="has-text-right">
        {{ element.value}}%
      </td>
    </tr>
    {% endfor %}

  </tbody>
</table>

Each of these categories are described more below.

{% include anchor.html level="h4" text="Participation" %}

Participation includes pass/fail assignments such as participating in surveys, discussions on Piazza, in-class exercises, attending labs, lab exercises, and participating in other on-campus or off-campus CS events. *Late submissions are not accepted for participation assignments.*{:.has-text-danger}

{% include anchor.html level="h4" text="Quizzes" %}

Quizzes are sometimes given unannounced at the start of class, but students will often be given an opportunity to retake those quizzes. Quizzes will be conducted on [Canvas]({{ site.data.info.links.canvas.link }}), and the answers will automatically be released after the quiz deadline. Because of this, *late submissions are not accepted for quizzes.*{:.has-text-danger}

{% include anchor.html level="h4" text="Exams" %}

There will be two exams. The exams are *not* comprehensive. Each exam will have a retake opportunity where students may earn back a small fraction of the points missed on the original attempt. See [Important Dates](#{{ "Important Dates" | slugify }}) for the exact exam and exam retake dates.

Instead of a final exam, students will have a final project graded during finals week. A signup sheet will be posted towards the end of the semester. If you have travel plans during finals week, please confirm your travel dates first with the instructor.

Students must receive a C letter grade or higher on at least one exam (including retakes). See the [Pass Requirements](#{{ "Pass Requirements" | slugify }}) for more.

{% include anchor.html level="h4" text="Homework" %}

Homework programming assignments are assigned on a semi-weekly basis, and usually due the following week. Students may work on these assignments during their lab session, allowing them to get immediate help from the teacher assistants.

Homework will receive a late deduction if submitted after the deadline as follows:

  - &ndash;10% deduction for homework submitted 15 minutes to 24 hours after the deadline
  - &ndash;20% deduction for homework submitted 24 hours to 48 hours after the deadline

*Homework submitted over 48 hours after the deadline will not be graded.*{:.has-text-danger} However, students may request extra credit opportunities on [Piazza]({{ site.data.info.links.piazza.link }}) The lowest homework grade will also be dropped at the end of the semester.

{% include anchor.html level="h4" text="Projects" %}

Programming projects place an emphasis on code quality&mdash;it is not enough to achieve correct results. Each project must pass several functionality tests and then undergo multiple rigorous code reviews checking for specific criteria, such as proper encapsulation and generalization, efficiency, and maintainability.

We use a **mastery learning** approach with projects: students must perfect the current project before moving on to the next project. The final project grade will depend on when and how many projects are completed.

Each project grade is split into two components: functionality (evaluated with automated software tests) and design (evaluated with one-on-one code reviews). The project functionality must be passed before the code review may be passed, students must pass code review for each project sequentially, and may only have one review appointment per week.

There are only 2 hard deadlines for projects: the project cutoff 1 deadline before the withdraw deadline, and the project cutoff 2 deadline at the end of the semester. See the [Pass Requirements](#{{ "Pass Requirements" | slugify }}) for details.


{% include anchor.html level="h2" text="Course Policies" class="is-uppercase" %}

This section includes miscellaneous policies specific to this course, including communication, attendance, credit hours, cheating, and more. These policies are *in addition* to the standard USF policies included later.

{% include anchor.html level="h3" text="Communication Policy" %}

Most course-related communication will be handled using [Piazza]({{ site.data.info.links.piazza.link }})&mdash;a FERPA-compliant Q&amp;A platform that supports public, anonymous, and private posts. When making posts on Piazza, please keep the following in mind:

  - Make a **public post** when appropriate. This lets us answer questions once for all students. You can **post anonymously** if you are uncomfortable with attaching your name to a post or a response. When posting anonymously, your classmates will not be able to see your identity, but instructors will still be able to see your name (necessary to give you credit for participation and ensure everyone is following the code of conduct).

  - Do not post code on Piazza. If you have a question regarding your specific code, please commit and push your code to your GitHub repository and [post a link](https://help.github.com/en/articles/creating-a-permanent-link-to-a-code-snippet). That ensures only those with access to your repository (instructor and teacher assistants) will see your code.

  - Make posts regarding grades or specific solutions **private** to the instructor and teacher assistants. When making private posts, they should always be marked as visible by both the instructor and teacher assistants so there is no confusion.

In addition to [Piazza]({{ site.data.info.links.piazza.link }}), the instructor will also use [Canvas]({{ site.data.info.links.canvas.link }}) to notify students of missing assignments or warn about low grades. Both the instructor and teacher assistants will use [Github]({{ site.data.info.links.github.link }}) for project-related communication. You may also ask for help in-person during office hours, lectures, or lab sessions. These are the *only* officially approved channels of communication for contacting the instructor or teacher assistants.

**Under no circumstances should you reach out to the teacher assistants via any unapproved communication channel.**{:.has-text-danger .has-text-weight-normal} Instructors and teacher assistants must provide all students equal opportunity for course-related help. Using unapproved communication channels creates an unfair advantage over other students and will be treated as a violation of the [Student Conduct Code](https://myusf.usfca.edu/fogcutter).

*For example, it is appropriate to use text messages to invite a teacher assistant to lunch as friends. It is NOT appropriate to start asking that teacher assistant questions about the course during that lunch! It is also NOT appropriate to directly text message course-related questions to that teacher assistant, even if you are friends and were able to get help from them before. You can, however, ask that teacher assistant for help during official office hours.*
{:.has-text-grey .is-size-7}

{% include anchor.html level="h3" text="Announcements Policy" %}

All announcements will be posted on [Piazza]({{ site.data.info.links.piazza.link }}). All students are expected to enroll in Piazza and monitor the announcements in a timely manner. This includes any changes to the lecture, lab, office hour, or deadline schedule.

{% include anchor.html level="h3" text="Attendance Policy" %}

Students are expected to be on-time to all classes to minimize disruption. Attendance is mandatory for all exams, quizzes, guest speakers, and in-class exercises. Exam dates will be posted on the course schedule.

Attendance is mandatory for all one-on-one code review appointments. Students must be on-time to these appointments. If a student arrives more than 5 minutes late, the appointment will be canceled. *Students risk a grade penalty for repeated canceled or missed appointments.*{:.has-text-danger}

{% include anchor.html level="h3" text="Credit Hour Policy" %}

All courses must comply with the [Credit Hour Policy](https://myusf.usfca.edu/sites/default/files/usf_credit_hour_policy_0.pdf), which states:

> One unit of credit in lecture, seminar, and discussion work should approximate one hour of direct faculty instruction and a minimum of two hours of out-of-class student work per week through one 15-week semester.

As this is a 4 credit course, students must spend a **minimum** of 8 hours of out-of-class work per week to earn a passing (D&ndash; or higher) letter grade. To earn a C or higher letter grade (as required for the CS major), students should expect to spend closer to **10 to 20 hours per week** on projects, homework, and participation assignments.

*Think of this class like a part-time job. If you do not put in the time, you will not make it to the final project. Many students do not pass due to poor time management!*{:.has-text-grey .is-size-7}

{% include anchor.html level="h3" text="Cheating Policy" %}

All students are expected to know and adhere to the University's [Honor Code](https://myusf.usfca.edu/academic-integrity/). In short, students must never represent another person's work as their own. Examples of honor code violations include (but are not limited to):

  - Copying and pasting code (especially without attribution) from the web
  - Copying from another student (past or current)
  - Having anyone other than yourself complete your work (including tutors)
  - Working too closely with others such that your code no longer represents an individual contribution
  - Sharing your solutions with others (either directly or indirectly)

Keep in mind that unauthorized collaboration or discussion that results in the same or very similar code indicates that you have not placed enough independent work into your submission and is a violation of the honor code, regardless of whether you directly copied any code!

**Flagrant or repeat violations of the honor code will result in an F in the course, [a report to the Academic Integrity Committee (AIC)](https://myusf.usfca.edu/academic-integrity/review-process), and a report to the Dean.**{:.has-text-danger} At the discretion of the instructor, a less severe penalty may be imposed for minor or first offenses. This is at the sole discretion of the instructor and any violation may result in an F in the course.

{% include anchor.html level="h3" text="Policy Exceptions" %}

Exceptions to most course policies are made only in the case of verifiable exceptional circumstances. This includes medical emergencies, mental health and well-being crises, or family-related emergencies. Extensions must be arranged prior to the original deadline unless in case of extreme emergency (such as an emergency room visit).

*Have travel plans for a family event (such as a wedding or graduation) or academic/professional conference (such as Grace Hopper or an internship interview)? Contact the instructor ahead of time to make arrangements. Keep in mind you will likely be asked to submit assignments early versus getting an extension. Please note exceptions will not be made for other events (such as concerts, comic cons, and so on).*
{:.has-text-grey .is-size-7}


{% include anchor.html level="h3" text="Getting Help" %}

A good rule of thumb is to seek help after you have been stuck for an hour. There are many ways to get help with this class:

  - Ask questions on [Piazza]({{ site.data.info.links.piazza.link }}). Most questions receive a response in under 24 hours (sometimes within 30 minutes). You may figure out your problem before you get a response, but then you can delete your question or mark it as solved.

  - Ask questions during the instructor office hours. Office hours are first-come first-serve and there is lots of seating (including power outlets for charging).

  - Ask the teacher assistants for help during lab sessions or their office hours. All of the teacher assistants for this course took CS 212 previously with Professor Engle.

  - Ask a tutor for help at the [CS Tutoring Center](http://tutoringcenter.cs.usfca.edu/). Many of the tutors took CS 212 previously (and many of them also took it with Professor Engle). However, even tutors that did not take CS 212 may be able to help. Sometimes, it just helps to talk about your code with someone (see [rubber duck debugging](https://en.wikipedia.org/wiki/Rubber_duck_debugging)).

  - Ask your classmates for high-level help or hints, but be careful! To avoid violating the cheating policy and honor code, make sure you never share code with your classmates or look at the code of your classmates.

If you are feeling generally overwhelmed (including emotionally) and need advice, do not hesitate to reach out to the instructor. Since office hours can be crowded at times, you are welcome to schedule an appointment with the instructor via [Piazza]({{ site.data.info.links.piazza.link }}) to chat in private.

<hr>

{% endcomment %}
