# Thesis Templates

In this git repository you will find a template to write your bachelor’s or Master’s thesis at the Technical University of Munich. You might choose between two templates:

- Latex. This is the conventional latex template.

- Lyx. Lyx is an WYSIWYG (What You See Is What You Get) graphical interface on top of latex. It compiles your project using latex without you having to know the latex syntax. However it still allows you to write latex code if you prefer. See: [Lyx Website](https://www.lyx.org/). *Note: you can open the invididual files, but to compile the entire thesis you should open the "__Thesis.lyx" file.*

# Thesis Structure

## Chapter 1 - Introduction

Introduce the topic of your thesis by describing the background / context.

### 1.1 Problem

What problem are you addressing? Justify why it is relevant to solve this problem? To whom is this problem relevant. Suggestion: ask your supervisor for a few related research papers and extract a few arguemtns asa bullet points describing the problem. Share those arguments with your supervisor per email.

### 1.2 Motivation

What are you doing and if not obvious why does it have the potential to solve or help solve the problem mentioned? Note: if the problem and motivation sections are only one or two paragraphs long, consider merging them under the Introductin directly (without subsections).

### 1.3 Outline

List the content of each chapter briefly.

## Chapter 2 Background (optional)

Describe any technique you might be using later on in your thesis (e.g. wavelet analysis) or the Activity Recognition chain.

## Chapter 3 - Requirement Specification

In this chapter, you describe the concepts, taxonomies and relationships of the application domain. Note: Make sure that the whole chapter is independent of the chosen technology and development platform. If you are going to develop a system to detect lacrosse goalkeeper training exercises using a peak detection algorithm to detect high energy in the signal, you will want to model the stick, the sensor, how the sensor is attached to the stick, the signal, how the signal looks like when the player performs an exercise, where the peak is located. 

### 3.1 Related Work

Try to group works done by others to solve the same problem. For example, to automatically detect lameness in cows, researchers have already tried using vision techniques, pressure sensitive mattresses and attaching sensors to cows. You should make it clear how your work relates to the related work.

Example citation in Lyx: [Bruegge2004software]. You can copy paste this citation, click on the citation and select the paper you want to cite from the list.

### 3.2 Visionary Scenarios

Describe 1-2 visionary scenarios here, i.e. a scenario that would perfectly solve your problem, even if it might not be realizable.

### 3.3 Functional Requirements 

List and describe all functional requirements of the ideal system. Note that you might not implement the entire system within your thesis. Still, describe the requirements for that system. The short title should be in the form ``verb objective''.

1. [Detection]. The system should classify the pig activities including: eating, resting, walking, running, 
2. [Name]. Short Description.
3. [Name]. Short Description.

### 3.4 Non-Functional Requirements 

List and describe all nonfunctional requirements of your system. Also mention requirements that you were not able to realize.

1. [Robustness]. The sensor might be prone to bites from pigs. Therefore, the sensor should be water-proff and able to resist high amounts of force being applied to it.
2. Category. Short Description.
3. Category. Short Description.

### 3.5 Use Case Model

This subsection should contain a UML Use Case Diagram including roles and their use cases. If the system is initiating most of the use cases in the background (e.g. tracking user activities), then you can have a Virtual Coach actor initiating the use cases. Give a name to the system other than 'System' and a name to the actor other than 'Actor', such as 'Goalkeeper'.

### 3.6 Analysis Object Model

This subsection should contain a UML Class Diagram showing the most important objects, attributes, methods and relations of your application domain including taxonomies using specification inheritance. Do not insert objects, attributes or methods of the solution domain. Make sure to describe the analysis object model thoroughly in the text so that readers are able to understand the diagram. Also write about the rationale how and why you modeled the concepts like this.

### 3.7 Dynamic Model (optional)

This subsection should contain dynamic UML diagrams. These can be a UML state diagrams, UML communication diagrams or UML activity diagrams. Make sure to describe the diagram and its rationale in the text. Do not use sequence diagrams.

## Chapter 4 System Design

The goal of this chapter is to show an overview of the system, in particular including subsystems and how these subsystems are mapped to a hardware device. If you investigated different technologies, you can address their tradeoffs in this section (relate them to the non-functional requirements).

### 4.1 Subsystem Decomposition

Describe the architecture of your system by decomposing it into subsystems and the services provided by each subsystem. You can use UML components or subsystems for each subsystem. You should add a short description of what each subsystem / component does.

### 4.2 Hardware/Software Mapping

This section describes how the subsystems or components are mapped onto existing hardware and software components. The description is accompanied by a UML deployment diagram.

*Note: you can merge the subsystem decomposition and Hardware Software mapping by using a deployment diagram that uses nodes (cubes) to describe the hardware devices software components contained inside the hardware nodes.*

## Chapter 5 - Object Design

Here goes the core of your project. Describe what algorithms and data structures you used so that your work can be reproduced. You can organise this chapter wth a section for each subsystem you identified in the previous section, and a subsection for each relevant object (e.g. Segmentation Algorithm) you used.

## Chapter 6 - Evaluation

If you did an evaluation / case study, describe it here. Add images to give a better feel about what you actually did (e.g. how you collected the data at the hospital).

### 6.1 Design

Describe the design / methodology of the evaluation and why you did it like that. E.g. what kind of evaluation have you done (e.g. how did you chose your users and why? what where your subjects instructed to do? How long did they do it? How much data did you collect? If you used machine learning, be sure to describe your data set (how many instances of each class did you have), ideally with a table.

### 6.2 Results

Present the results without interpreting them. If you are working on a machine learning application, provide a table including Accuracy, Precision, Recall, F1-Score and the confusion matrix.

### 6.3 Discussion

Interpret the results presented. The main goal is to justify whether your approach would be suitable for solving the problem you addressed in the Introduction.

### 6.4 Limitations

Describe limitations and threats to validity of your evaluation, e.g. possible overfitting, issues in the way how the data was collected that might lead to different behavior in real life (also mention how they could be solved in the future).

## Chapter 7 - Conclusions

Recap shortly which problem you solved in your thesis and discuss your contributions here.

7.1 Future Work 

What do you think could give better results?
*Note: if the future work is one or two paragraphs long, consider merging it into the Chapter 9 (eliminate the Future Work subsection).*
