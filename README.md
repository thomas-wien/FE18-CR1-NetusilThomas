
# Code Review 1

Welcome to your 1st CodeReview! After learning CSS3, it is time to create your first CodeReview and mobile-friendly website! 

You will need to achieve more than 60 points to pass this CodeReview successfully.  

You will be graded according to the results achieved. Please see the number of points for each task below.  

The grading system has the following rules: 

Up to 60 points = red 

Between 61 and 79 = yellow 

Over 80 = green 

You can submit your solution (as GitHub project link) until Saturday 18:00:00. 

 
# Project description: 

You will create a mobile-friendly website for one of the most popular food blogs out there, fittingly named “Food blog”. 

Please examine the image below and use it as a guide in order to create your index.html for the desktop resolutions: 

 

 

 

For this CodeReview, the following criteria will be graded: 

    (5 points) Create a GitHub Repository named: FE18-CR1-YourName. Push the files into it and send the link through the learning management system (lms). See an example of a GitHub link below: 

https://github.com/JohnDoe/repositoryname.git 

Please remember to set your repository to private and invite codefactorygit as a collaborator!  

    (05 points) Correct usage of the HTML structure. Make sure to use proper semantic elements and not only div elements. Use the right code indentation as well. 

    (10 points) Use CSS selectors (classes and/or IDs) to style your web page. Make sure the classes have useful and proper names. Stick to the English language for it. 

    (10 points) Use SASS/SCSS tools to style your website.

    (15 points) Correct usage of Flexbox and/or Grid (when necessary). The elements should be displayed according to the design given, respecting the columns and rows.

    (20 points) Using positioning attributes, place the images with their respective overlays as in the example (hint: remember that for an absolute position child element, the parent element must use position relative). Alternatively, you can use background-image attribute instead.

    (20 points) Correct usage of Media Queries. For mobile resolution of =< 480px, you should use the second guide template. 

    (10 points) Create a "recipe of the month" page and include the link in the top navbar. Fill this page with individual content. Be creative and choose a delicious recipe. 

    (5 points) The contact-us link in the footer must be linked to https://codefactory.wien/en/contact-en/

Bonus Points: 

    (10 points) Create a webpage for the About link in the footer and provide your design/layout solution for this additional page. It must have a navbar, a middle section with the main content about the Food-blog and a footer.

    (10 points) Create a Media Query for tablets. For this option, as the tablet resolution is wider, two columns should be able to fit in the screen. *Research what is the most popular tablet breaking point.

NOTE: Bootstrap won't be accepted in this code review. It is important to follow the structure of the layout, including the placement of all elements. The cropping of the images, the font size and font family are not important. 

You can use sources such as Unsplash or Pixabay to find the best pictures for this CodeReview.

Focus on how the pictures are positioned in the 2 images: 3 columns layout for the desktop vs. 1 column layout in the mobile version.



Submission status
Submission status 	Submitted for grading
Grading status 	Graded
Due date 	Saturday, 28 January 2023, 6:00 PM
Time remaining 	Assignment was submitted 4 hours 24 mins early
Last modified 	Saturday, 28 January 2023, 1:35 PM
Online text 	

https://github.com/thomas-wien/FE18-CR1-NetusilThomas.git
Submission comments 	
Comments (0)
You can still make changes to your submission
Feedback
Grade 	100.00 / 100.00
Graded on 	Tuesday, 31 January 2023, 1:29 PM
Graded by 	Picture of Riola LamaRiola Lama

# Feedback comments 	

Hi Thomas, well done on your first code review. You managed to accomplish all the requirements. The code is well organized and I also saw that you created separated variables for the breakpoints., very clever of you.
Please find some of my suggestions below:
-for the media, you can specify the media and then inside include the elements that you want to change for ex. 
@media screen and (min-width: $media_mobile-min) and (max-width: $media_mobile-max) {
.grid {
grid-template-columns: repeat(1, minmax(100%, 1fr));
}
figure {
flex-basis: 1;
}
}
and please do keep your media queries at the end, what you can do is create a separate file and then declare all the media in there. Inside the main css file you can import them by including them at the end, so they will override every style from previous files.
- In order to remove the horizontal scroll when you start shrinking the browser to mobile devices, inside the ul add a flex-wrap property and set it to wrap, so your elements will wrap when you move to smaller devices

Overall good job, let me know if you have any questions :)
