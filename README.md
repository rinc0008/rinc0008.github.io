To create the portfolio, I use custom CSS and Bootstrap throughout all the website mostly for align items, modify some margins, add buttons, cards and to make grid layouts in the following pages: About, Illustration and Web design.  Each page of my portfolio website gave me challenges to surpass to make it look how I wanted and at the end l am learning with every project how to diagnostic each problem and find multiple possible ways to solve them. I list some challenges that I found with the solution I gave to them:

1.	The most difficult challenge was to create a 3-position navigation bar, being in the desktop, a side nav bar.
-	For the desktop and mobile the 'a' where all aligned center, in the tablet the elements were split, the text at the right side and the logo at the left.
-	I tried use the 3-position side bar from 3wschools as starting poiny because was the more similar to my muck-up but the problem with this, was that it does not use progressive enhancement because it has media queries for tablet and mobile, so it was not mobile first. So, I reverse in the media queries the important elements that make the .nav-bar move with properties such a ‘display:block; position;fixed;’ for desktop or ‘display:flex’ in mobile or ‘float:none; text-align: center;’ for mobile.
-	I had my nav bar in the 3 positions now, but the logo was centered all the time (good for mobile and desktop but not for tablet. So, I start using Bootstrap using class to declare that those elements are part of the nav bar, implementing dropdown-dividers and most important in the 'img' class add ‘d-block’ which send the logo right to the left corner, now all the screens had the logo in the left! (My mistake) let’s make this responsive ‘d-md-block d-lg-inline’ by adding display block in medium screen size (≥768px) and display inline for long screens (≥992px) it will reset and follow the customize css which send them to the center in mobile and desktop.

2.	Find the effective way to import video files that moves with the container size. Which format is the better for showcase the video work? 
-	If importing the video in html I will have to also create the controls for each one and the user will have to activate one per one, I did not want this, I want the video to repeat and play automatically without any controls. It is just visual and with no sound. So, I went for .gif format. And as those all has specific aspect ratio will not move with the screen when shrinking or enlarge in vertical containers.
-	As I want them to fit all the container space, I decided to import them as a background-image in the custom css and use them as a cover. I create empty divs and gave them a height and an auto width or some time the other way around, or just assigns them to a grid row/column or grid area in the case of the ‘video page’. When put in columns the container takes the height of the grid-item in the same row, which works perfectly responsive. 

3.	Once I find the solution for the last challenge, I was ready to commit the changes and pull/push to GitHub... But I could not, the Gif files were too big (around 100mb each). How can I convert the files and be able to upload them to github?
-	The maximum file size allowed was 25mb, so what I did was export short gifs around 2-3 secs, allowing them to showcase a good amount of content. Then I compressed the files being careful not to lose much image quality, and upload directly in the repository ‘image’ folder.

4.	I wanted to use the buttons directly with bootstrap, but I add an 'a' parent and when validating the code it was an error, I tried the other way around and was invalid too, so I eliminate the 'button' tag and put the button bootstrap classes in the 'a' which then, I put into a 'div' with an invented class to target all buttons this to align them depending on the screen size. 


Resources List:

All the images and videos are my own content.
	The videos used in the video edition gif are from pexels.com and videezy.com


Fonts from Google fonts:
-	Annie use your telescope:
https://fonts.google.com/specimen/Annie+Use+Your+Telescope
-	Raleway:
https://fonts.google.com/specimen/Raleway?query=rale


Bootstrap: 

-	Card groups:
https://getbootstrap.com/docs/4.0/components/card/
-	Carousel:
https://getbootstrap.com/docs/4.0/components/carousel/
-	Buttons:
https://getbootstrap.com/docs/4.0/components/buttons/
-	Forms:
https://getbootstrap.com/docs/4.0/components/forms/
-	Align:
https://getbootstrap.com/docs/4.0/utilities/text/#text-alignment
-	Color:
https://getbootstrap.com/docs/4.0/utilities/colors/
