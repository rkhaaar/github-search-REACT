# github-search-REACT

This project objective was to produce a single web app that would deliver and show the search user/users on GitHub and relocating you into their GitHub repo or profile in case you wanted. I did this project for a job opportunity as a challenge in order to show what I could do and learn by studying react.
I never had any contact before this project with react so for me was very challenging specially when you don’t know where to start and what a component is.
So first step was to buy an Udemy course of react for beginner’s which I didn’t finish in time because I just had a week to show them my code. After I realised was almost impossible if you not a genius to do it in one week (if you never seen it), my second step was to search on web for various examples using react where they implemented the GitHub api. 
After this I start to select the information I wanted and how to organize it in order to make my challenge.

Basically I used the REACT - ROUTER - DOM  library in order to implement dynamic routing in order to keep my web app as a single web app.

<img width="741" alt="mrouting codeshot" src="https://user-images.githubusercontent.com/115631586/212302681-b6217b29-ff80-4070-915a-ccb2804a7e63.png">


On the screenshot above you can see that I’ve called createRoot in order to create a react root for displaying content inside the browser which will be provided by the bit of code bellow.

<img width="725" alt="routing codeshot" src="https://user-images.githubusercontent.com/115631586/212302846-51792852-3573-4a55-a0f1-025d7a939893.png">



On the screenshot above we can find the function responsible of the routing, by wrapping up the content with BrowserRouter and they defining the multiple route’s. The first Route with the path ‘/‘ will render the layout component named ‘Home’. The next now will inherit and add to the parent route, being redirect to the user page that will display the user clicked on the results search. Because we don’t know which user will that be, i’ve used a parameter ,the symbol ‘:’ defines it as a parameter ready to render path based on the login information.


The other library I used was AXIOS in order to handle my http requests, on this case the requests to the GitHub api.
<img width="456" alt="axios codeshot " src="https://user-images.githubusercontent.com/115631586/212302911-ee701651-2f97-492d-813c-634e29e93cd6.png">

On the screenshot above you can see that I’ve defined a default url in order to help me access later to the GitHub api.

<img width="551" alt="axios codeshot 1" src="https://user-images.githubusercontent.com/115631586/212302963-34a7e753-eb4f-4591-800d-25485ed7addf.png">


On the screenshot one example in how the I’ve used axios to fetch the users information, on this case inside an effect hook, since the base url is already defined this http get request will be added to the default.


How the project is organized:

The Landing page is ‘Home.js’ where you could search the user you wanted to find, when you search it will generate and fill under the search field all the users obtained by your search, they are generated on ‘User.js’ that you can find on the folder ‘ui’. Since there’s a possibility of several user’s showing up, I’ve introduced pagination in order to organise better the results. 
In case you click a user on the results, a new page will open being this page ‘User.js’ that you can find on the folder ‘pages’. On this page you’ll find more detailed information regarding the user you clicked, in case you want to see their repositories or profile on GitHub, you can just click on them and you’ll be redirected to page you requested.
I’ve also made this project to be Responsive, meaning it’s possible to see it regarding the window size always with a similar design. I’ve done this by dimensioning almost all the css using percentages in order to make it more flexible.

Functionalities Checklist:
- [x] The Search page;
- [x] The User page;
- [x] User profile picture;
- [x] User name;
- [x] User number of repositories;
- [x] Redirecting to the User profile desired.
- [x] Responsive web design;



