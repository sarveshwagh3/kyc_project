PROBLEM STATEMENT -
"KYC Document Identification and Extraction of UID"


ABOUT THE APPLICATION -
Our application takes a decent image of any KYC document (Aadhaar Card/ PAN Card/ Passport Card/ Voter ID Card/ Driving Licence Card/ NREGA Card) as the input and outputs the type of the KYC document (classification) and the Unique Identification Number (UID) on the KYC Document (Extraction). For example - If one inputs an image of his/her PAN Card the output is "This is a PAN Card with UID ^^^^^####^" where "^^^^^####^" is the UID.

Along with this, a "Heuristic Correctness Index" in percentage would be output. This heuristic score represents the code's confidence that the input image is indeed of the type output by it. An index of 100% would mean that there is a high probability that the input image is of the type output by the code.

The execution time on the website varies from 5 seconds to 25 seconds depending on the input image. The accuracy of our application is certainly above 99% for a decent image taken on any smartphone. The algorithm for string searching and double-checking has been designed by us completely (read the PPT).

Pytesseract library was used for OCR and Open-CV library for preprocessing.

A mobile application was also built using the same flask application on Android Studio. The image input to the mobile application is stored on Firebase storage and later passed on to the Azure server. The output from our flask application is displayed within 15 seconds on the mobile screen. To reduce the execution time the accuracy was compromised a bit for the mobile application. The mobile application does not handle big input images (>=500 kb) which the website can very easily handle.


LINK TO WEBSITE -
http://52.172.157.10:5000/ This website is hosted on Azure Cloud service.


LINK TO PPT (IF YOU WISH TO KNOW MORE) -
https://docs.google.com/presentation/d/1HtX04BIkOnobuLp1rApgckJswSZOmiR65BkMqCCnik8/edit


FILES -
"app.py" file contains the flask application 
"Kulchau KYC App.apk" file is the mobile application apk
"templates" folder contains the HTML files
