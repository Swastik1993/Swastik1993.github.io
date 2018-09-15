---
layout: post
title:  "BRIDGEi2i interview experience"
date:   2018-09-09 10:30:00 +0530
categories: interview
---
So I recently got a job from __BRIDGEi2i Analytics Solutions__ through the campus placement and thought of sharing my interview experience so that others may find it useful. The job role(s) offered were:- 
* Data Analyst - for undergraduate students 
* Business Analyst - for postgraduate students 

### Round 1 - Online Test 

As usual there is the online test as the first step of the selection process. I don't remember the exact order but the online test had 5 sections: 
* quantitative ability, 
* logical reasoning, 
* statistics, 
* programming theory and 
* pseudo code output.  


There were 90 questions and 120 mins to answer them (No negative marking). The questions were not exactly tough but it was difficult to answer all questions as the time was short. I left 5 questions un-attempted. 

I wasn't confident of the fact that I would qualify for the second round since I didn't know how others had done, but I had some hopes. There were about 60 candidates shortlisted from our college and 108 in total (including people from NIT Rourkela and Calcutta University) for the GD round.  

### Round 2 - Group Discussion 

Before starting the group discussion round a small presentation was given by the company representatives. The group discussion round was pretty interesting we were given a case study. We were each given a sheet of paper in which the case study was defined. I will give a brief idea of how the problem was defined as I don't remember the exact description by heart.  

In the year 1992 Reid had won the election by a 10% margin. He had some characteristic traits that were given like... personality, outlook, focus, democrat, liberal, etc and the classes of people which voted for him in 1992 such as... elderly, academic groups, urban families, NGOs, etc.  
Now in 1998 the competitor is Ensign a new guy, he also had some personality traits such as... radical, republic, divorced etc. and the sections of people who supported him like... young, suburban families, new entrants, etc.  
However this time(1998) Reid less confident about his victory so he has hired you, as an analyst to understand the scenario and draw conclusions about the election results.  
The population details of 1992 and 1998 were given and was pretty detailed. Each sections of the population was given in % values to indicate the population growth within the time period. For example the data was given as follows:-  

class of people | population in 1992  (2.5 million) | population in 1998  (3.4 million)
--- | --- | ---
Male | 49% | 51%
Female | 51% | 49%
Elderly | 44% | 40%
New entrants | 34% | 42%
Urban families | 42% | 39%
Suburban families | 34% | 40%

There were about 15 to 20 such rows and I don't remember all the sections and percentage values.  

Based on the given data the questions were:-  
* Who stands at a better position to win the election?
* What are the key differences between the previos election and this election?
* What can Reid do to be confident or make sure that he has the upper hand in the election?  

Out of the 108 candidates only 30 or 40 were selected for the final round.  

### Round 3 - Technical Interview + HR  

I was interviewed by one of the co-founders of the company, who was also the CTO and another developer (she didn't ask any questions though). I have to say that this was one of the best technical interview experiences I ever had in my life. The interviewers were so friendly and encouraging that it didn't felt like I was giving an interview.  

So I entered the room and went upto the table and handed over my resume to the developer and greeted them with a handshake. Then after I sat down the interview started - 

* Q: Let's start with your introduction. Tell me about yourself.  
A: I am Swastik Biswas, my parents own a garment store. I completed my 10th and 12th standard from Salt Lake School, Kolkata. Thereafter I went to Acharya Institute of Technology, Bangalore to study Computer Science and Engineering for my undergraduate degree. While studying I had also served as an intern at ITC Infotech, Bangalore. After completing my graduation I took the GATE exam and here I am at Jadavpur University pursuing my Masters degree in Computer Science and Engineering working on Volumetric Medical Image Segmentation as my masters thesis.  

* Q: Tell me about your current research project.  
A: Well it's basically a novel FCM clustering approach to segment regions of interest within MRI and CT scan images. I am using the dataset from Brainweb to segment the grey-matter, white-matter, cerebrospinal fluid and bone structure. The data is in rawb format and it has 181 such images packed within it, which are first extracted and then processed serially. I have to run the algorithm for 10 such datasets.  

* Q: How is the FCM working?  
A: It works very similar to the k-means clustering approach. First we choose a number of clusters in my case it is 4 as I am interested in segmenting 4 specific regions; grey-matter, white-matter, cerebro-spinal fluid(csf) and background. Then I assign membership values randomly to each data point for being in the clusters. Finally I have to repeat the steps of computing the centroid for each cluster center and each membership values of the data points until the algorithm has converged (that is, the coefficients' change between two iterations is no more than the given sensitivity threshold).  
I am using a gaussian distribution function for calculating the distance between any two data point and incorporated shanon entropy in the original cost function for a statistical comparision with the original cost function.  

* Q: What are the tools you are using for your project?  
A: I am not using any additional tools at all. The entire project is made using C and it's standard library functions.  

* Q: So you are working with images right? (I nodded). There is growing buzzword of Deep Learning and Image Analysis... have you got any idea about this?  
A: Yes sir, I have had some experience of working on Deep Learning using images. Specifically I had implemented a small CNN for classifying objects from real-time videos. It was my under graduate project.  

* Q: To a completely non-technical person how would you explain the CNN architecture?  
A: (I had to draw the CNN architecture and explain to him what is a convolution, activation function, how each node in the network works and why CNN is a good choice for object classification).  

* Q: Now I am going to give you a picture (he drew a picture of a car on a road). Your problem is to color each of the areas in the picture (the car, sky, road) with a different color. How do you do it?  
A: If I have a set of pictures of cars already, then I can use those images to slide through the original picture and look for maximal matching. And then I check these results to find if any of them have crossed over a certain threshold say 80% match, to conclude the region as a car and apply any color to identify it. Then I can simply put a different colour for the region below the coloured car and above it. It will definitely not be a good looking picture as some regions may not be properly coloured but it solves the problem to some extent using simple image processing. It can definitely be improved should I continue? (by this time the interviewer had shown his satisfaction to my answer so I stopped).  

* Q: What did you do during your internship at ITC Infotech?  
A: I had worked on a project for Advanced driver-assistance systems in which the task was to specifically segment out regions of interest from the dashcam of a car based on driver's interest (I cannot put more details here because of copyrights).  

* Q: I see you have mentioned Keras and Tensorflow on your resume. How comfortable are you at using them?  
A: I had used Keras on Tensorflow backend for the first time when doing my undergraduate project on deep learning. After that I have used it for some 2-3 kaggle competitions so I can say I am fairly familiar with it, but I do need to check the documentation while coding.  

* Q: I see you have worked on a lot of problems but most of them are specific to images. How would you apply your knowledge for the company if I tell you that the data we use dosen't contain any images at all?  
A: It's not like that I know only images. I am just passionate about Computer Vision and thats why I have worked on that matter the most. Images are just a representation of data that helps us to visualize things easily but that data can be anything. If I have the data with me I can obtain *information* about the core aspect of the problem and using that information I can have analysis and visualizations to help me understand the data, to have an *insight*. Based on those understandings I can prepare results or model the solutions for the problems such that it can create an *impact* for the company. I am still young and I want to learn and hopefully if I have the chance to work on a variety of data I will improve my knowledge more and I believe you will definitely help in that process.  

* Q: Do you have any questions in your mind that you wish to ask?  
A: (During the presentations the interviewer had mentioned that they deal with gigabytes and terabytes of data) I would really like to know that with the amount of data that you have what do you do to handle that data. I mean like you have a specific data center or do you only use cloud services and if so what are the compnents. - This was my question.  
The interviewer told me that they have a small data center and they used cloud services too specifically AWS to solve the problems. It is mainly dependent on the problem statement what kind of data preprocessing may be required and how it should be stored like in files or a relational model, etc. They also use MongoDB and Cassandra among other products for their data.  

After this they told me that by the end of day they will announce the list of selected candidates. I came back home and at night our placement coordinator called to tell me that I was among the list 11 of selected students.  

