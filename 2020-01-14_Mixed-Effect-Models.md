Mixed Effects Models and other notes from the session
================
Lukas Schmid
9 1 2020

# exams

## example code

  - everybody got the best grade

## 48-hours exam

### formalities

  - we have to send in five to ten pages (PDF)
  - Henrik will not read the any more pages
  - we will be sent the code at 10:00 on Saturday, 1st of March
  - we have to send the code back until 10:00 on Monday, 3rd of March
  - there will be an additional 5% on the grade for writing a
    [Haiku](https://ja.wikipedia.org/wiki/%E4%BF%B3%E5%8F%A5) about the
    data
  - our task is to find the most important patterns of the data, “What
    is the most important message in the data?”
  - there will be different datasets (four to nine) which everyone of us
    will be assigned to (groups of three to four people)

> I never said you should work together. But it would be stupid not to.
> *(Henrik von Werden)*

### content and structure

  - tests can be used, but we do not have to explain how they work
    statistically
  - how to structure the code
      - tell a story about the data\!
      - Chan suggests to look at Lukas S.’s code about the
        treering-datasets: communicate what questions you have asked
        yourself when you looked at the code
  - general starting point: nature of the dataset, descriptive
    statistics, formulate assumptions and main questions (Henriks ideal
    number for research question is five)
  - focus on specifics that help you answer your question
  - leave all possible specifications at the default ones provided by
    RStudio

### evaluation criteria that Henrik

  - steps of analysis that do not contribute to (one of the) question(s)
    that were posed will be counted towards a bad evaluation
  - results should answer the question (or draw the conclusion that the
    question can not be answered by the data)
  - graphics have to adhere to common standards (labels, legends, etc.);
    they can also be altered in size
  - plots should not reflect the person’s skills, but try to present
    information as precisely as possible
  - try to maintain a balance between the different parts (= answers to
    the different questions)

# writing code coherently

  - some code was well explained, other not so much
  - we need a way to make sure that shared code works on different
    machines:
      - **send the plain code (.R or .Rmd)** and a **PDF generated from
        R Markdown**
      - additionally, everyone can send the report in any other format
        (e.g. .html) for more interactive documents

# Mixed Effects Models

  - continuation of generalised linear models
  - they are very complicated and we might never need them
  - baseline example: How does a drug work, not how a drug works *on a
    specific person*, even though drugs do have varying effects on
    different people.
  - way it works: takes in different factor variables (e.g. different
    hospitals) as input
  - e.g. medical studies try to eliminate the influence of general
    health (smoking, sports, obesity)
  - these factors are called random factors (even though they are not
    technically ‘random’, only in relation to the question)
  - in R, there are certain packages to calculate mixed effects models
    (sometimes called multilevel models): `lme4` for multilevel modeling
    in general, `lmerTest` for p-values in these, and `sjstats` for some
    tools that surround mixed effects models
  - for a visualisation (coded in R), see
    <http://mfviz.com/hierarchical-models/>
