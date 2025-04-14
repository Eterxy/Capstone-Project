"# Capstone-Project for CSCI 400" 

### Project Webpage can be accessed here [Capstone](https://eterxy.github.io/Capstone-Project/)

The excel sheet used to contain the form input <a href = "https://docs.google.com/spreadsheets/d/1mVq43J9HVCdcfet0E04cEMRWxmHWQ5MRCKyph6x3p5g/edit?usp=sharing">is here </href>

 For our project, before we create the phishing email we first need to create the background that will give the phishing email legitimacy, allowing more victims to fall for the email. So first, we opened up the legitimate John Jay email password reset website in order to retrieve the information required to create the fraud version of it. On the website, we inspect the webpage which will open up the built-in web-developer tools and on the inspector tab we will see the code that makes up the webpage. 

All that html code can be directly copied from the webpage into your own html file, but we have to make slight modifications to it as the website uses php files instead of html files which meant that the redirection links are all directed to other php files that exist on the server and cannot be accessed by us. So we edited the code such that instead of passing an event when the student button is clicked, it instead redirects the user to another html code we have created that is in the same file location.


Now the webpage we created will have a similar function as the original webpage as it will redirect the user to the webpage that corresponds to the button clicked. However with only the html code, our webpage will look nothing like the original webpage as the original one has css code that defines the style the webpage has. In order to get the same style the original webpage has, we can change the tab in the web-developer tools to style-editor which will contain the css code.

Once we have the css code copied to a folder in the same file location as our html code, we just need to edit the html code so that it utilizes the css code using link rel:”stylesheet” which creates a relationship between the html file and the css file such that the css file is imported to the html file as a stylesheet.


Once the css file is added and connected to the html code, we open up the fraud website we created and compare it to the original one. Unless you pay very close attention you will find it hard to spot any differences and as the intended target of our phishing attack rarely uses the webpage, it will be even harder for them to notice that they opened up a fake website. For the rest of the webpages we created, we simply took the html code from the actual webpage and rewrote the redirection link so that it is redirecting the user to another html file we have in the location.

Then on the student password reset page, we changed the name of the html form to “submit-to-google-sheet” and for the submission button, instead of continuing to redirect the user it will simply have the name “submit”. Below the html form, a script is added in that will take all the input values that the user gave and post them into the google excel sheet that the url is pointing to. 


We would then use the data we collected from the user to reset the password on the actual John Jay email reset website, gaining access to the user’s email. The last part was creating an email prompt that we will use to send to John Jay students. Phrases like “You have 3 days” and “It has been 180 days” that John Jay students are accustomed to seeing will help give the email authenticity and are less likely to raise suspicion.

	Although our phishing tactic works, there is one way we thought of to improve it. Originally, when we get the victim’s information from the excel sheet, we have all that we need to gain access to the email. The dilemma is the victim also knows that they have been hacked when they go to log into their John Jay email and is denied. This inturn raises alarms and as hackers limits our flexibility to a smash and grab tactic before the alarms are raised. To combat this problem, we would create another page that will ask for the old and new password from the victim. After obtaining the information, we will manually change their password with the “new” password they use so when they log into their email, they would not know that we have access to their email. This improvement provides flexibility for long term phishing while staying undetected. 





References
How to Recognize and Avoid Phishing Scams. (2022, October 25). Consumer Advice. https://consumer.ftc.gov/articles/how-recognize-and-avoid-phishing-scams 
Irwin, L. (2023). How to Spot a Phishing Email: With Examples. IT Governance UK Blog. https://www.itgovernance.co.uk/blog/5-ways-to-detect-a-phishing-email 
Phishing Scams. (2021, July 16). Federal Trade Commission. https://www.ftc.gov/news-events/topics/identity-theft/phishing-scams 
What is a phishing attack? | IBM. (n.d.-a). https://www.ibm.com/topics/phishing?utm_content=SRCWW&p1=Search&p4=43700068223686516&p5=p&gclid=EAIaIQobChMIut6W642F_wIVoRxlCh0BeAHEEAAYASAAEgIVevD_BwE&gclsrc=aw.ds 
“Phishing Chain” Image: https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.valimail.com%2Fguide-to-phishing%2F&psig=AOvVaw1ZLIId9ms1mgxUMheZl2aJ&ust=1684768627885000&source=images&cd=vfe&ved=0CBAQjRxqFwoTCJjV1q7ahv8CFQAAAAAdAAAAABAE
