# Programming_CA1_Python_Data_Acquisition_Preprocessing_Pipeline

Link To my Github repositor: https://github.com/Aneesh-Kalita-10617414/Programming_CA1_Python_Data_Acquisition_Preprocessing_Pipeline.git

Webscraping is the process of collecting information from Webpages. The information may be text data or even Images, videos or audio files. The process can be manual but it is generally practise to automate the process by writing Python code. In this assignment we will use the request library to fetch data from webpages and the Beautiful Soup package to parse through the HTML trees to extract information.

The requests library is installed. It is used to send HTTP requests to wepages. Get requests are used to fetch data from the webpage whereas Post requests are used to send forms or data ro webpages.

A function is created to fetch the URLs of the required Webpages.
The fetched Website is a Musical instrument shopping website named www.thomann.de

Function is created to fetch all the necessary Guitar features from the Webpages

In this function, at first we will call the get_url function to get the URL list containing strings of the two main Webpage URLs. Then an empty list is created to append the features of each Guitar saved in respective dictionaries. A loop is created to run through the two main webpages. HTTP requests are sent to these Two webpages to retreive the rensponse object which contains all the required information in the webpage. The content of the server's response is saved into a variable src.
With each request we make, after saving the response content, the Request Connection to server is closed. This prevents overloading and crossing the threshold connection duration time authorised by server.
The response content contains an HTML tree. It has to be parsed by a parser. In our case, we use the Beautiful Soup Package to parse through the HTML trees and the lxml parser.

A nested for loop is created to go through each guitar in the main Webpage to fetch the Manufacturer, Model, Price and Availability of the 50 Guitars. Further, in another nested for loop, we go thorugh each Guitar Webpage individually to fetch theeir URL and using BeautifulSoup fetch all the remaining features from that nested webpage

Further, documentation is included in the Code file for reference.
