This Project was developed in Smart India Hackathon 2018 and is currently under deployment in Indian Railways.
Problem Statement:
Indian Railways has online system of customer feedback in suggestion. Customers can give their feedback on website, mobile application as well as through social media. Since the number of feedback is large, machine reading of the content and classification among various departments, zonal and regional offices can help in quick transfer of such feedback to the concerned officials for immediate redressal. A solution need to be developed for such a utility.
Solution Proposal
1.	Approach
Indian Railways has an online system of customer feedback which is a ‘Customer Complaint-cum-Suggestion’ portal. The volume of this data is very large which is generated through the website, mobile application and through social media. Every feedback needs to be directed to the concerned official for immediate redressal, for which each feedback has to be analyzed and classified into types. This will be done by a machine learning algorithm that will be trained with a data set so that it efficiently recognizes the type of complaint/suggestion and the concerned official. This not only skips the step of manually reading each feedback to determine where to forward the message, but also makes the process time reduce from hours to a few seconds for the large volume of data.
2.Types of Complaints Incorporated
	The model developed by us takes care of the complaints from every possible source. Following are the types of complaints which are generally received by Railways:
(a)	Text Extraction from image of post complaints using handwriting recognition: An app was developed for this purpose using computer vision API, which could recognize the text from handwritten posts.
(b)	Feedbacks and Complaints on Social Media like Facebook, Twitter: Any tweet tagging railway ministry was fetched into the Python Script using Tweepy API and appropriate action was taken then, depending on whether the tweet was a suggestion or Complaint.
(c)	Recording Complaint via Voice Input: The Railway Passengers who don’t use social Media can also file their Complaint using their voice. An app was developed for this purpose.
(d)	Text Message Complaints and Feedback on Helpline Number: Customers can also text their complaints on the provided Railway Helpline Number.
3.Key Features of Model for Complaints
•	The Complaints from the Running Train having high priority was tried to resolve on the upcoming next station.
•	Complaints can be in any language.
•	Complaints were rightly classified inspite of the spelling and Grammatical Mistakes.
•	Irrelevant Complaints were discarded.
4.Classification Features
•	The Complaints were classified on the basis of their priority into corresponding Department, Region and Zone so that they could be dealt accordingly.
•	Suggestions and Feedbacks were Separately Classified.
•	The record of each Complaint was stored in a database along with the username, complaint id, source of complaint, corresponding classifications and Remarks.
•	An App was developed for each department which received the classified Complaint. The App had facility to provide the feedback to the server, i.e. whether or not the complaint was resolved. Also, if it was wrongly classified, then also the server would be notified. The record of these complaints was kept for the purpose of Self-training of the Machine Leaning Model so that these mistakes can be further avoided and hence the Model would grow better with increase in volume of data.
•	Similar types of Complaints were Clustered together so that similar notification can be issued to the complaints belonging to same cluster. This would save the processing time.
5. Analysis:
•	A comparative Analysis of the various machine learning models used was prepared and the one having highest accuracy was chosen.






