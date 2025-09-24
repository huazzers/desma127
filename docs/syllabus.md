
<!--jump to anchor tag adjusted to header height offset-->
<script>
// Get the header element
let header = document.querySelector('header');

// Get the height of the header
document.querySelectorAll('a[href^="#"]')
.forEach(function (anchor) {
    anchor.addEventListener('click', 
    function (event) {
        event.preventDefault();

        // Get the target element that 
        // the anchor link points to
        let target = document.querySelector(
            this.getAttribute('href')
        );
        
        let headerHeight = header.offsetHeight*2;
        
        let targetPosition = target
            .getBoundingClientRect().top - headerHeight;

        window.scrollTo({
            top: targetPosition + window.scrollY,
            behavior: 'smooth'
        });
    });
});

window.onload = function(e){
    var cell = document.getElementById('component-site-name');
    var caseId = cell.innerHTML;
    cell.innerHTML = '';
    var link = document.createElement('a');
    link.href = '../';
    link.appendChild(document.createTextNode(caseId));
    cell.appendChild(link);
}
</script>

# 📜 Syllabus

---

Broad 4230<br/>
Tuesdays and Thursdays, 2 p.m. - 4:50 p.m.

**INSTRUCTOR**<br/>
Office hours: Tuesdays 12:30 p.m. - 1:30 p.m.; By appointment only.<br/>
Email: huazzers@ucla.edu

**TEACHING ASSISTANT**<br/>
Office hours: Thursdays 12:30 p.m. - 1:30 p.m.; By appointment only.<br/>
Email: yo0na@ucla.edu

## Course Description
This course explores traditional and experimental animation techniques that are central to 2D and 3D interactive digital projects and video games. 

Coursework develops skills and concepts that are integral to animation workflows and game engine animation systems, including traditional animation principles, 2D sprite animation, rigging 2D and 3D game objects, and character controller implementation. 

Students will experiment with common and alternative input methods for real-time interactivity. Readings, screenings, and in-class gameplay sessions will supplement lessons throughout the quarter.

---

## Learning Outcomes
Throughout this course, tutorials and studio time center on introducing animation workflows and honing technical skills that are useful for interactive projects. Students will…

- Learn classic animation principles and how to design animated assets suited specifically for the Unity game development platform.
- Activate and navigate 2D sprite and rig-based animations using a mouse, keyboard input (and more)
- Develop low-poly modeling, rigging, and animation skills in Blender to make CG assets for Unity implementation
- Use the Animation System program simple object interactions in Unity

Lectures, coursework, and readings focus on concept-building, examining artworks, and the performative implications of interfacing, using physical controllers, and using tracked input.

---

## Course Outline

### Unit 1: 2D Techniques and Mouse/Keyboard Inputs

> **Week 1**
</br>Introduction to animation principles, loops, and asset creation for 2D workflows.
> 
> **Week 2-3**
</br>Introduction to Unity: How to set up interactions with 2D sprite and rig-based animations using mouse and keyboard input.
> 
> **Week 4** </br>Project 1 Presentation

### Unit 2: 3D Techniques and Custom Inputs

> **Week 5-9**
</br>Working with CG modeling, rigging, and experimenting with custom controllers and input methods.
> 
> **Week 10** </br>Project 2 Presentation

---

## Assignments and Grading
> See [*How To Submit*](./how-to-submit.md) on instructions for submitting Unity projects

This is a **5 unit** upper division studio class. Expect to work/attend 6 hours a week in class and 9 hours a week outside of class.

### Course Breakdown
> * **Project 1: 30%**
> * **Project 2: 30%**
> * **Reading / Media responses: 20%**
> * **Engagement / Participation / Communication: 10%**
> * **Attend an Event in the Game Lab: 10%**
> 
> * **Extra Credit:** <br> Seek out an interactive game, performance, installation, or gallery work. Go see it in person and tell me about your experience.

### Evaluation Criteria
#### Projects

In general, your projects should:

1. show consideration for **topics discussed in class**;
* demonstrate **at least one skill** covered in class; 
* be creatively ambitious enough to **push your technical and conceptual practice** from your current level of skill and comfort; and 
* must be **completed by the specified deadline**. 

<br>

We will evaluate your projects based on:

> * **Timely submission**</br>Did you submit your project on time? (see [*Late Work*](#late-work) for more details.)
> * **Completion of Project Deliverables**</br>Does your project meet the requirements of the assignment?
> * **Conceptual investment / development**</br>What are you trying to say with your work? Are you engaging with these ideas at a critical, in-depth, or personal level? 
> * **Project scope / aesthetic and technical ambition**</br>Are you doing the bare minimum, or are you pushing yourself technically and/or aesthetically? 
> * **Attention to detail and craft**</br>Does the project run? Are there unintended bugs, glitches, etc.
 
#### Reading / Media Responses

You will be assigned readings and interactive projects that are related to this course, accompanied by some questions you'll be asked to repsond to. 

#### Engagement / Participation / Communication

Your engagement and participation grade involves:

* your **timely attendance** in class *(see [Attendance Policy](#attendance-policy) for more details)*;
* your **active contributions** in class activities and studio critique; and
* your **responses to technical questions and discussions** during class.

Most importantly, you'll be graded on your ability to **promptly and clearly communicate your needs with us throughout class**. If you will be late or absent to class, have questions, need direction, or are struggling with your work, email us so we can help you. Always CC the TA on emails unless you need to speak with me confidentially. 

#### Attendance Policy

**If you are more than 5 minutes late to class (ie. 2:05pm**), you will be marked as **late**. 

**Two (2) late marks** results in **an unexcused absence**.

Unexcused absences will lower your grade. **More than three (>3) unexcused absences will result in an automatic fail**, and must be addressed on a case-by-case basis. 

**If you need to be late or excused, you should inform me AND the TA before class begins**. It is also your responsibility to arrange alternative plans with me and the TA for any work you've missed from being absent (eg. attending office hours, sharing project updates, etc.) 

#### Late Work
**On the day the project is due:**

* Projects should be ready to play **prior to the beginning of class**.
* Project files and documentation should be **submitted by 11:59PM** the same day.

**If you anticipate that you won’t be able to complete the work by the due date, please contact us *before* the due date so we can discuss options.**

#### Technology Policy

Related to your [engagement and participation](#engagement-participation-communication) grade, **all phone and laptop usage should only be for class-related work.** 

If you need to use them for anything else during class time, please step outside the classroom and return when you're done. 

#### Appropriation, Fair Use, and Generated Content

**You are expected to develop your own assets for your project submissions.** Please don’t use appropriated 3D models, motion capture data, images, or music that you do not have explicit permission to use -- and don't copy games and other projects.

With Unity C# scripts, you're encouraged to **start with the examples available in the tutorial notes**, and then modify them as necessary for your own projects. If there's anything you've taken from somewhere else, note it down as a comment or in your submission so we can help decode what you're doing. **No writing code using AI from scratch.** 

The use of prompt-based AI generation programs, including but not limited to ChatGPT, DALLE, Stable Diffusion, and Midjourney, is **strictly not allowed** in this class. There are [many other reliable solutions and resources](resources.md) available to you, please use this opportunity to explore them.

If you're planning to borrow or generate assets from anywhere else, please consult the instructor beforehand AND be able to justify your decision for doing so. While developing early stage prototypes, it is acceptable to use placeholder assets.

**No credit will be awarded for plagiarised work.** All submitted projects should be original and developed within the duration of this class. Remember to acknowledge / cite your tools and sources appropriately in your submission.

---

## Campus-wide resources and information

### Land Acknowledgement

> The University of California, Los Angeles occupies the ancestral, traditional, and contemporary Lands of the Tongva and Chumash peoples. Our ability to gather and learn here is the result of coercion, dispossession, and colonization. We are grateful for the land itself and the people that have stewarded it through generations. While a land acknowledgment is not enough, it is the first step in the work toward supporting decolonial and indigenous movements for sovereignty and self-determination. Read more about what land you’re occupying: [https://native-land.ca/](https://native-land.ca/) 

Other resources on land repatriation: 

* [**UCLA Mapping Indigenous LA**](https://mila.ss.ucla.edu/) -- an online archive of a storymapping research project about indigenous Los Angeles peoples, histories, and geographies from past and present.
* [**California History (Winter 2023), Respecting the Ancestors: On Repatriating American Indian Remains**](https://online.ucpress.edu/ch/article/100/4/3/197683/Respecting-the-AncestorsOn-Repatriating-American) -- 2023 essay report on the history of repatriating indigenous peoples remains (mostly a lack thereof), including UC-specific case studies. 
* [**Decolonization is not a metaphor**](https://www.semanticscholar.org/paper/Decolonization-is-not-a-metaphor-Tuck-Yang/9e908da74710ecdcac794a847564939390008374) -- article on what is unsettling about decolonisation as a caution against the loose use of the term in advocacy and scholarship. 

### Know your Rights - ICE on Campus

This classroom is a place that honors the experiences of all students regardless of nationality, immigration status, or other factors. I understand that this quarter is likely to be a particularly challenging time for students navigating issues related to immigrant and international student rights. I pledge instructional flexibility including **negotiable project grade weighting**, **online documentation of course materials**, and **options for remote participation**. You do not need to disclose your immigration or visa status to me to access these flexibilities. If you would like to request these accommodations, just let me know.
 
Students who have concerns about their legal rights as immigrants or international students may seek resources via the [Undocumented Students Program](https://usp.ucla.edu/), [IDEAS](https://www.instagram.com/ucla_ideas/), and the [Dream Resource Center](https://labor.ucla.edu/our-projects/dream-resource-center/). You may also approach me for advice or help connecting to these resources. 

In particular, the [**Undocumented Student Program Legal Services**](https://usp.ucla.edu/legal-services) provides legal advice and representation for undocumented UC students or UC students with undocumented family members. You can reach Gina Pech, the Supervising Attorney for the Legal Services Team at [**gpech@saonet.ucla.edu**](mailto:gpech@saonet.ucla.edu). If you are detained, or need urgent immigration related legal counsel, you may call Ms. Pech at [**424-832-0977**](tel:+14248320977). 

Additionally, here is the most up-to-date document containing [**advice and resources for international students at UCLA**](https://drive.google.com/file/d/1x8_zUP5-PRtXQETFz7bOnbXlMp5Sf_2L/view), including precautionary measures, who to contact in an ICE encounter, and what to do if your visa status is compromised.


### Commitment to Diversity & Safer Spaces
We understand the classroom as a space for practicing freedom; where one may challenge psychic, social, and cultural borders and create meaningful artistic expressions. To do so we must acknowledge and embrace the different identities and backgrounds we inhabit. This means that we will use preferred pronouns, respect self-identifications, and be mindful of special needs. Disagreement is encouraged and supported, however our differences affect our conceptualization and experience of reality, and it is extremely important to remember that certain gender, race, sex, and class identities are more privileged while others are undermined and marginalized. Consequently, this makes some people feel more protected or vulnerable during debates and discussions. A collaborative effort between the students, TA, and instructor is needed to create a supportive learning environment. While everyone should feel free to experiment creatively and conceptually, if a class member points out that something you have said or shared with the group is offensive, avoid being defensive; instead approach the discussion as a valuable opportunity for us to grow and learn from one another. Alternatively, if you feel that something said in discussion or included in a piece of work is harmful, you are encouraged to speak with the instructor or TA. 

*(Statement adopted from voidLab at [https://github.com/voidlab/diversity-statement](https://github.com/voidlab/diversity-statement))*

### Undergraduate Writing Center

The [Undergraduate Writing Center](https://uwc.ucla.edu/) is a free service for all UCLA students, providing one-on-one appointments. Appointment topics include course papers, capstone projects, senior thesis papers or application materials (resumes, CVs, statements of purpose or cover letters).

### Inclusivity Statement

UCLA’s Office for Equity, Diversity and Inclusion provides resources, events and information about current initiatives at UCLA to support equality for all members of the UCLA community.  I hope that you will communicate with me or your TA if you experience anything in this course that does not support an inclusive environment.  You can also report any incidents you may witness or experience on campus to the Office of Equity, Diversity and Inclusion on their website [https://equity.ucla.edu](https://equity.ucla.edu). 

### COVID-19
It is important that everyone stay safe and avoid coming to class if you have any concerns about your health status.

If you find that external struggles and/or COVID related challenges are affecting your ability to attend class, please reach out to us. We want you to be successful in the class, but we care about your well-being more than anything else. Open communication with us is most important in this regard, please let us know if you're sick and/or require additional accommodations.

Students must adhere to the current campus directives related to COVID-19 mitigation, and refusal to do so may result in the student being asked to leave the classroom or referred to the Dean of Students. For more information about COVID-19 requirements on campus, please visit: [https://covid-19.ucla.edu/information-for-students/](https://covid-19.ucla.edu/information-for-students/). 

### Center for Accessible Education (CAE)
The UCLA Center for Accessible Education (CAE) is responsible for ensuring students with documented disabilities have access to an inclusive, supportive learning environment. Students with disabilities or other needs requiring academic accommodations should speak with me as early in the quarter as possible to be sure they get the support they need.

Students needing academic accommodations based on a disability should contact the Center for Accessible Education (CAE) at (310) 825-1501 or in person at Murphy Hall A255. When possible, students should contact the CAE within the first two weeks of the term as reasonable notice is needed to coordinate accommodations. For more information visit <a href="https://www.cae.ucla.edu">www.cae.ucla.edu</a>. 

### Academic Integrity and Information on Student Conduct
UCLA is a community of scholars. In this community, all members including faculty, staff and students alike are responsible for maintaining standards of academic honesty. As a student and member of the University community, you are here to get an education and are, therefore, expected to demonstrate integrity in your academic endeavors. You are evaluated on your own merits. Cheating, plagiarism, collaborative work, multiple submissions without the permission of the professor, or other kinds of academic dishonesty are considered unacceptable behavior and will result in formal disciplinary proceedings usually resulting in suspension or dismissal. As specified in the [UCLA Student Conduct Code](https://www.deanofstudents.ucla.edu/studentconductcode), violations or attempted violations of academic dishonesty include, but are not limited to, cheating, fabrication, plagiarism, multiple submissions or facilitating academic dishonesty. When a student is suspected to have engaged in academic dishonesty, Academic Senate regulations require that the instructor report the allegation to the office of the Dean of Students. For more information, see the [UCLA Student Conduct Code](https://www.deanofstudents.ucla.edu/studentconductcode).

### TITLE IX
UCLA prohibits gender discrimination, including sexual harassment, domestic and dating violence, sexual assault, and stalking. If you have experienced sexual harassment or sexual violence, there are a variety of resources to assist you.

#### Confidential Resources
You can receive confidential support and advocacy at the CARE Advocacy Office for Sexual and Gender-Based Violence, 1st Floor Wooden Center West, [CAREadvocate@careprogram.ucla.edu](mailto:CAREadvocate@careprogram.ucla.edu), (310) 206-2465. Counseling and Psychological Services (CAPS) also provides confidential counseling to all students and can be reached 24/7 at (310) 825-0768.

#### Non-Confidential Resources
You can also report sexual violence or sexual harassment directly to the University’s Title IX Coordinator, 2241 Murphy Hall, [titleix@conet.ucla.edu](matilto:titleix@conet.ucla.edu), (310) 206-3417. Reports to law enforcement can be made to UCPD at (310) 825-1491. These offices may be required to pursue an official investigation.

Faculty and TAs are required under the UC Policy on Sexual Violence and Sexual Harassment to inform the Title IX Coordinator—A NON-CONFIDENTIAL RESOURCE—should they become aware that you or any other student has experienced sexual violence or sexual harassment.

### Psychological Health, Well-Being and Resilience
UCLA is renowned for academic excellence, and yet we know that many students feel overwhelmed at times by demands to succeed academically, socially and personally.  Our campus community is committed to helping all students thrive, learn to cope with stress, and build resilience. Remember, self-care is a skill that is critical to your long-term success.  Here are some of the many resources available at UCLA to support you:

* **Counseling and Psychological Services (CAPS)**: [https://www.counseling.ucla.edu/](https://www.counseling.ucla.edu/) Provides counseling and other psychological/mental health services to students. Walk-in hours are Monday-Thursday 8am-4:30pm and Friday 9am-4:30pm in John Wooden Center West. Crisis counseling is also available 24 hours/day at (310) 825-0768.
* **Ashe Student Health and Wellness Center**: [http://www.studenthealth.ucla.edu](http://www.studenthealth.ucla.edu) Provides high quality and accessible ambulatory healthcare and education by caring professionals to support the academic success and personal development of all UCLA students.
* **Healthy Campus Initiative (HCI)**: [https://healthy.ucla.edu](https://healthy.ucla.edu) Provides links to a wide variety of resources for enhancing physical and psychological well-being, positive social interactions, healthy sleep, healthy eating, healthy physical activity and more.
* **Campus and Student Resilience**: [https://www.resilience.ucla.edu/](https://www.resilience.ucla.edu/) Provides programs to promote resilience and trains students to help support their peers.
* **UCLA Recreation**: [https://www.recreation.ucla.edu/](https://www.recreation.ucla.edu/) Offers a broad array of services and programs including fitness, yoga, dance, martial arts, meditation, sports, and much more.
* **Equity, Diversity and Inclusion**: [https://equity.ucla.edu/](https://equity.ucla.edu/) Committed to providing an equal learning, working and living environment at UCLA and supports a range of programs to promote these goals campus-wide.
* **UCLA GRIT Coaching Program**: [https://www.grit.ucla.edu/](https://www.grit.ucla.edu/) GRIT stands for Guidance, Resilience, Integrity and Transformation. In this program, UCLA students receive individualized support from trained peer coaches to manage stress, foster positive social connections, set goals, and navigate campus resources.

#### Resources for Students Dealing with Financial Stress 

* **Economic Crisis Response**: [https://www.studentincrisis.ucla.edu/Economic-Crisis-Response](https://www.studentincrisis.ucla.edu/Economic-Crisis-Response) provides support and guidance to students who have self-identified, or are identified by UCLA faculty or staff, as experiencing a financial crisis that impacts their academic success at UCLA.
* **Bruin Shelter**: [http://www.bruinshelter.org/](http://www.bruinshelter.org/) provides a safe, supportive environment for fellow college students experiencing homelessness by fostering a collaborative effort between universities, community-based organizations, and service providers.
* **The CPO Food Closet**: [http://www.cpo.ucla.edu/cpo/foodcloset/](http://www.cpo.ucla.edu/cpo/foodcloset/) provides free food for any UCLA student who may be experiencing hunger and/or struggling to attain food due to financial hardships.