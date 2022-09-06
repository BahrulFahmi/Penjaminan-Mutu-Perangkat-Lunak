Chapter 1

# The software quality challenge

    Chapter outline

    1.1  The uniqueness of software quality assurance

    1.2 The environments for which SQA methods are developed

        Summary

        Review questions

        Topics for discussion

<div style="text-align: justify">Two basic questions should be raised before we proceed to list the variety of
subjects and details of the book:

1.  Is it justified to devote a special book to software quality assurance (SQA)
or, in other words, can we not use the general quality assurance textbooks
available that are applicable to numerous areas and industries?

2.   Having decided to develop specialized books for software quality assurance, at which of the various environments of software development, from
amateurs’ hobby to professionals’ work, should we aim our main efforts?
Put simply, what are the unique characteristics of the SQA environment?

The objective of this chapter is to answer these questions by exploring the
related issues.

After completing this chapter, you will be able to:
<ul>
■ Identify the unique characteristics of software as a product and as production process that justify separate treatment of its quality issues.

■ Recognize the characteristics of the environment where professional software development and maintenance take place.

■ Explain the main environmental difficulties faced by software development and maintenance teams as a result of the environment in which 
they operate.</ul>

### 1.1 The uniqueness of software quality assurance

“Look at this,” shouted my friend while handing me **Dagal Features’s**
Limited Warranty leaflet. “Even **Dagal Features** can’t cope with software
bugs.” He pointed to a short paragraph on page 3 of the leaflet that states
the conditions of the warranty for **AMGAL**, a leading Software Master product
sold all over the world. The leaflet states the following:
<ul>
LIMITED WARRANTY

**Dagal Features** provides no warranty, either expressed or implied, with
respect to **AMGAL’s** performance, reliability or fitness for any specified
purpose. **Dagal Features** does not warrant that the software or its documentation will fulfil your requirements. although **Dagal Features** has
performed thorough tests of the software and reviewed the documentation, **Dagal Features** does not provide any warranty that the software and
its documentation are free of errors. **Dagal Features** will in no case be
liable for any damages, incidental, direct, indirect or consequential,
incurred as a result of impaired data, recovery costs, profit loss and third
party claims. the software is licensed “as is”. the purchaser assumes the
complete risk stemming from application of the **AMGAL** program, its
quality and performance.

If physical defects are discovered in the documentation or the CD on
which **AMGAL** is distributed, **Dagal Features** will replace, at no charge,
the documentation or the CD within 180 days of purchase, provided
proof of purchase is presented.</ul>

“Is the AMGAL software really so special that its developers are incapable
of meeting the challenge of assuring a bug-free product?” continued my
friend. “Do other software packages limit their warranties in the same way?”

Though **Dagal Features** and AMGAL are fictitious, an examination of
the warranties offered by other software developers reveals a similar pattern.
No developer will declare that its software is free of defects, as major manufacturers of computer hardware are wont to do. This refusal actually
reflects the essential elemental differences between software and other industrial
products, such as automobiles, washing machines or radios. These differences can be categorized as follows:

1.  **Product complexity.** Product complexity can be measured by the number of operational modes the product permits. An industrial product,
even an advanced machine, does not allow for more than a few thousand modes of operation, created by the combinations of its different
machine settings. Looking at a typical software package one can find
millions of software operation possibilities. Assuring that the multitude
of operational possibilities is correctly defined and developed is a major
challenge to the software industry.

2.  **Product visibility.** Whereas the industrial products are visible, software
products are invisible. Most of the defects in an industrial product can be
detected during the manufacturing process. Moreover the absence of a
part in an industrial product is, as a rule, highly visible (imagine a door
missing from your new car). However, defects in software products
(whether stored on diskettes or CDs) are invisible, as is the fact that parts
of a software package may be absent from the beginning.

3.  **Product development and production process**. Let us now review the
phases at which the possibility of detecting defects in an industrial product may arise:
<ul>

(a) **Product development.** In this phase the designers and quality assurance (QA) staff check and test the product prototype, in order to
detect its defects.

(b) **Product production planning.** During this phase the production
process and tools are designed and prepared. In some products there
is a need for a special production line to be designed and built. This
phase thus provides additional opportunities to inspect the product,
which may reveal defects that “escaped” the reviews and tests conducted during the development phase.

(c) **Manufacturing.** At this phase QA procedures are applied to detect
failures of products themselves. Defects in the product detected in the
first period of manufacturing can usually be corrected by a change in
the product’s design or materials or in the production tools, in a way
that eliminates such defects in products manufactured in the future. </ul>

In comparison to industrial products, software products do not benefit
from the opportunities for detection of defects at all three phases of the
production process. The only phase when defects can be detected is the
development phase. Let us review what each phase contributes to the
detection of defects:
<ul>

(a) **Product development.** During this phase, efforts of the development
teams and software quality assurance professionals are directed
toward detecting inherent product defects. At the end of this phase
an approved prototype, ready for reproduction, becomes available.
(b) **Product production planning.** This phase is not required for the software production process, as the manufacturing of software copies
and printing of software manuals are conducted automatically. This
applies to any software product, whether the number of copies is
small, as in custom-made software, or large, as in software packages
sold to the general public.
(c) **Manufacturing.** As mentioned previously, the manufacturing of
software is limited to copying the product and printing copies of the
software manuals. Consequently, expectations for detecting defects
are quite limited during this phase.</Ul>

The differences affecting the detection of defects in software products versus
other industrial products are shown in Table 1.1 and Frame 1.1.


It should be noted that significant parts of advanced machinery as well
as of household machines and other products include embedded software
components (usually termed “firmware”) that are integrated into the product. These software components (the firmware) share the same
characteristics of the software products mentioned above. It follows that the
comparison shown above should actually be that of software products versus other industrial products and non-software components of industrial
products that include firmware. Hereinafter, when mentioning software, we
will mean software products as well as firmware.


The fundamental differences between the development and production
processes related to software products and those of other industrial products
warrant the creation of a different SQA methodology for software. The need
for special tools and methods for the software industry is reflected in the professional publications as well in special standards devoted to SQA, such as
ISO 9000-3, “Guidelines for the application of ISO 9001 to the development, supply and maintenance of software”. This point is supported by the fact
that targeted guidelines have not been prepared by ISO for other industries, 

| Characteristik | Software Product | Other Industrial products |
| ---------- | --------- | ----------- |
| Complexity | Usually, very complex product allowing for very large number of operational | Degre of complexity much lower, allowing at mos a few thousand operational options | 
| visibility of product | Invisible to detect defects or omissions by sight (e.g. of a diskette or CD storing the software) | Visible product, allowing effective detection of defect by sight |
| Nature of development and production procces | Oppurtunities to detect defects arise in only one phase, namely product development | Oppurtunities to detect defect arise in all phases of development and production : <li> product development<li> product production planning<li> manufacturing |


    Frame 1.1 The uniqueness of the software development process

    ■ High complexity, as compared to other industrial products

    ■ Invisibility of the product

    ■ Opportunities to detect defects (“bugs”) are limited to the product
    development phase


and the only other targeted guidelines have been prepared for services (ISO
9004-2, “Quality management and quality systems elements: Guidelines for
the services”).

The great complexity as well as invisibility of software, among other
product characteristics, make the development of SQA methodology and its
successful implementation a highly professional challenge.</div>