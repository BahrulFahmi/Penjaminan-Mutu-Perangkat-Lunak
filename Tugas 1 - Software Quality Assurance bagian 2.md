# 1.2 The environments for which SQA methods are developed

<div style="text-align:justify">The software developed by many individuals and in different situations fulfills a variety of needs:
- Pupils and students develop software as part of their education.
- Software amateurs develop software as a hobby.
- Professionals in engineering, economics, management and other fields develop software to assist them in their work, to perform calculations, summarize research and survey activities, and so forth.
- Software development professionals (systems analysts and programmers) develop software products or firmware as a professional career objective while in the employment of software houses or by software development and maintenance units (teams, departments, etc.) of large and small industrial, financial and other organizations.

All those who participate in these activities are required to deal with software quality problems (“bugs”). However, quality problems in their most
severe form govern the professional software development.

This book is devoted, therefore, to defining and solving many of the software quality assurance (SQA) problems confronted by software developmentand maintenance professionals. However, all other types of software developers can find portions of the book applicable to and recommended for their own software development efforts.

Let us begin with the examination of the environment of professional software development and maintenance (hereafter “the SQA environment”), as it is a major consideration in the development of SQA methodologies and their implementation. The main characteristics of this environment are as follows:

1. **Contractual conditions.** As a result of the commitments and conditions defined in the contract between the software developer and the customer, the activities of software development and maintenance need to cope with:<ul><li>A defined list of functional requirements that the developed software and its maintenance need to fulfill.<li>The project budget.<li>The project timetable.</ul>
The managers of software development and maintenance projects need to invest a considerable amount of effort in the oversight of activities in order to meet the contract’s requirements.

2. **Subjection to customer–supplier relationship.** Throughout the process of software development and maintenance, activities are under the oversight of the customer. The project team has to cooperate continuously with the customer: to consider his request for changes, to discuss his criticisms about the various aspects of the project, and to get his approval for changes initiated by the development team. Such relationships do not usually exist when software is developed by non-software professionals.

3. **Required teamwork.** Three factors usually motivate the establishment of a project team rather than assigning the project to one professional:<ul><li> Other software development teams in the same organization.<li>Hardware development teams in the same organization.<li>Software and hardware development teams of other suppliers.<li>Customer software and hardware development teams that take part
in the project’s development.</ul>

4.  **Cooperation and coordination with other software teams.** The carryingout of projects, especially large-scale projects, by more than one team is a very common event in the software industry. In these cases, cooperation may be required with:<ul><li> Other software development teams in the same organization.<li> Hardware development teams in the same organization.<li> Software and hardware development teams of other suppliers.<li> Customer software and hardware development teams that take part
in the project’s development.</ul>
An outline of cooperation needs, as seen from the perspective of the
development team, is shown in Figure 1.1.

5. **Interfaces with other software systems.** Nowadays, most software systems include interfaces with other software packages. These interfaces allow data in electronic form to flow between the software systems, free from keying in of data processed by the other software systems. One can identify the following main types of interfaces:<ul> <li> nput interfaces, where other software systems transmit data to your
software system. <li> Output interfaces, where your software system transmits processed
data to other software systems.<li>Input and output interfaces to the machine’s control board, as in medical and laboratory control systems, metal processing equipment, etc.</ul>
<ul>
Salary processing software packages provide good examples of typical input and output interfaces to other software packages – see Figure 1.2. First let us look at the input interface. In order to calculate salaries, one needs the employees’ attendance information, as captured by the time

<img src = "figure 1.JPG">

clocks placed at the entrance to the office building and processed later
by the attendance control software system. Once a month, this information (the attendance lists including the overtime data) is transmitted
electronically from the attendance control system to the salary processing system. This information transmission represents an input interface
for the salary processing software system; at the same time it represents
an output interface to the attendance control system. Now, let us examine
the output interface of our system. One of the outputs of the salary
processing system is the list of “net” salaries, after deduction of the
income tax and other items, payable to the employees. This list, including
the employees’ bank account details, has to be sent to the banks. The
transmission of the list of salary payments is done electronically, representing an output interface for the salary processing system and an input
interface for the bank’s account system.

<img src = "figure 1.JPG"></ul>

6.   **The need to continue carrying out a project despite team member
changes.** It is quite common for team members to leave the team during
the project development period, whether owing to promotions to higher
level jobs, a switch in employers, transfers to another city, and so forth.
The team leader then has to replace the departing team member either
by another employee or by a newly recruited employee. No matter how
much effort is invested in training the new team member, “the show
must go on”, which means that the original project contract timetable
will not change.

7.  **The need to continue carrying out software maintenance for an extended period.** Customers who develop or purchase a software system expect
to continue utilizing it for a long period, usually for 5–10 years. During
the service period, the need for maintenance will eventually arise. In
most cases, the developer is required to supply these services directly.
Internal “customers”, in cases where the software has been developed
in-house, share the same expectation regarding the software maintenance during the service period of the software system.

The environmental characteristics create a need for intensive and continuous
managerial efforts parallel to the professional efforts that have to be invested in order to assure the project’s quality, in other words to assure the
project’s success.

A summary of the main characteristics of the SQA environment is shown
in Frame 1.2.

A significant amount of software as well as firmware development is not
carried out subject to formal contracts or formal customer–supplier relationships, as mentioned in the first two SQA environment characteristics. This
type of activity usually concerns software developed in-house for internal use

| Frame 1.2 | Summary of the main characteristics of SQA environment |
| -------------- | ------------------ |
| 1. |  Being contracted |
| 2. | Subjection to customer–supplier relationship |
| 3. | Requirement for teamwork |
| 4. | Need for cooperation and coordination with other development teams |
| 5. | Need for interfaces with other software systems |
| 6. | Need to continue carrying out a project while the team changes |
| 7. | Need to continue maintaining the software system for years |

or for marketing as software packages and in-house development of firmware. The relationships between the marketing department that initiates and
defines the qualifications of a new product and the respective in-house software development department often resemble a contract and customer–
supplier relationship. The same applies to internal requests for a new software system or for the upgrading of current software or firmware to be
implemented by the organization’s software department. Actual relationships between the internal “customers” and the development departments
are found to vary greatly when measured by a formal–informal scale. Some
managers claim that the closer the relationships to the formal form, the
greater the prospects for the project’s success.

## Summary
---
1. **The uniqueness of software quality assurance.**
<ul>The fundamental differences between software products (including firmware) and
other products are caused by the higher product complexity, by the invisibility of
software and by the nature of the product development and production process.
These differences create the need for an SQA methodology and tools for SQA that
will meet the special and different challenges for the development and operation of
quality assurance for software.</ul>

2. **The environments for which SQA methods were developed.**
<ul>The SQA methods and tools discussed in this book are specially aimed at the needs
of professional software development and maintenance, activities where quality
problems appear in their most severe form, and where the most painful losses are
expected. Therefore any method or tool to be applied is subject to the environmental characteristics of their activities, namely:
<ul>
<li> Contract conditions and commitments defining the contents and timetable.
<li> The conditions of the customer–supplier relationship, as realized by the need
for consultation with the customer and the acquisition of his approval.
<li> Teamwork requirements.
<li> Need for cooperation and coordination with other software and hardware development teams both internally and externally.
<li> Need for interfaces with other software systems.
<li> Need to continue carrying out a project when team members change.
<li> Need to conduct maintenance of the software system for several years.
</ul>
These environmental characteristics also apply to internal development of software
and firmware, though only informal contract or informal customer–supplier relationships exist in these cases. These characteristics demand that intensive and
continuous managerial efforts be expended in parallel to the professional efforts
that have to be invested in order to ensure the project’s quality or, in other words,
to assure the project’s success</ul>

### Review questions
---
1.  There are three major differences between software products and other industrial
products
<ul>
<ol>
<li> Identify and describe the differences.
<li> Discuss the ways in which these differences affect SQA
</ul>

2. It is claimed that no significant SQA activities are expected to take place during the
phase of production planning for software products.
<ul>
<ol>
<li> Discuss this claim.
<li>  Compare the required production planning for a new automobile model with the
production planning efforts required for a new release of a software product.
</ul>

3. Seven issues characterize the professional software development and maintenance environment.
<ul>
<ol>
<li> Identify and describe these characteristics.
<li>  Which of these environmental characteristics mainly affect the professional
efforts required for carrying out software development and maintenance projects? List the characteristics and explain why a professional effort is needed.
<li> Which of these environmental characteristics mainly affect the managerial
efforts required for carrying out software development and maintenance projects? List the characteristics and explain why such efforts are needed.
</ul>

### Topic For Discussion
---
1.  Educational systems are assumed to prepare the students to cope with real-life
conditions. Examine the procedural requirements of a software development project or final software project, and determine which of the requirements could be
considered as preparatory to professional life situations as discussed above.

2.  Referring to the seven environmental characteristics of software development and
121 The software quality challenge
maintenance, consider the characteristics of future software products, discussing
whether the professional and managerial burden of coping with these characteristics in future is expected to be higher or lower when compared with the current
performance of these activities.

3. The interfaces of a salary processing system are exhibited in Figure 1.2.
<ul>
<ol>
<li> Suggest what are the main benefits of applying computerized interfaces
instead of transferring printouts.
<li>  Give two additional examples where input interfaces are applied
<li> Give two additional examples where output interfaces are applied.
<li> Suggest additional situations where the use of input and output interfaces is
not applied and should be recommended.
<li> Would you advise all information transfers from one organization to another
be performed by computerized interface? Discuss the reasons behind your
answer.
</ul>

4.  The need to carry out work by a team demands additional investment in coordination of the team members. Discuss whether these managerial efforts could be
saved if the work were performed as a “one-man job”. 

5.  The need to carry out work by a team demands additional investment in coordination of the team members. Discuss whether these managerial efforts could be
saved if the work were performed as a “one-man job”.
<ul>
<ol>
<li>  Discuss whether a customer–supplier relationship is expected when the software developed is to be sold to the public as a software package.
<li>  Discuss whether a customer–supplier relationship is expected when software
is developed for in-house use, as in the case where a software development
department develops an inventory program for the company’s warehouses
<li>  Some managers claim that the closer relationships are to a formal pattern, the
greater the prospects are for the project’s success. Discuss whether implementing customer–supplier relationships in the situations mentioned in (1)
and (2) are a benefit for the company (referring to the internal customer and
supplier) or an unnecessary burden to the development team. 
</ul>

6.  It has been claimed that environmental characteristics create the need for intensive and continuous managerial efforts parallel to the professional efforts that
have to be invested in order to ensure the project’s quality or, in other words, to
assure the project’s success. Discuss the reasons behind this claim, including an
analysis of the managerial effort created by each of the SQA environmental characteristics.