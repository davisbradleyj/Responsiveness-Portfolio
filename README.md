# Responsiveness-Portfolio

## Technologies Used
- HTML - used to create elements on the DOM
- Bootstrap - used to style the page in place of css
- Git - version control system to track changes to source code
- GitHub - hosts repository that can be deployed to GitHub Pages

## Summary 
Using Bootstrap CSS Framework, I was able to create three html files to deploy this project, which features a page with a variety of links to the portfolio of projects that will be developed over the course of the next 11 weeks.  I was trying to be VERY strict with my use of the style sheet and media tags in the css folder - essentially forcing myself to exclusively use the styling present from GetBootstrap to acheive a recreation of the intended page, and adhering to their grid system to form the responsiveness of my work.  

For the most part, I was successful.  There appear to be some limitations with the ability to alter border thickness, and I am still trying to figure out how to "force" the navigation bar to push my page links to the right of the page.  I set up two columns, and had greater success having the "Name" box float to the right side of the page.  I have those lines present in the first section of code snipped below, but I felt the priority was assuring the mobile interface had the center justified content present.

The second snippet is a review of the logic in place to build out the portfolio screen, with the comments describing some of the rationale behind the choices made, and some ideas for further development as we gain more experience and a better understanding of JS to allow the page get some more punch.

While I had created a css page, I ultimately did not populate it with any tags or further styling, as I was challenging myselft to fully create the page using only the classes and elements available through GetBootstrap.

## Code Snippet

```html

<!-- This took the most time to figure out, and I basically started from scratch at one point as the design was not allowing me to have the two columns that make up the header stack on each other. I tried to start from the smallest screen level and was satisfied with the alignment of the name header and navigation links - at very wide screen levels, the alignment for the nav links is not fully right justified, but the aesthetics of not having a fully open top bar feels like it has some merit-->
<body>
  <header class="navbar d-flex flex-row justify-content-space-between sticky-top navbar-expand-sm mx-auto m-0 p-0 border-bottom border-secondary" style="border-width: 20px">
  <!-- The first of much tinkering with margins and padding throughout the document began with the header-->
    <div class="container mx-0 px-0">
      <div class="col-sm-6 text-center navbar-nav justify-content-center pr-0 float-sm-left">
  <!-- Info appears to be the most consistent color choice from the Bootstrap defaults, with white, light, and secondary used as needed for background and text choices throughout document -->
       <a class="navbar-brand text-white px-4 py-4 mb-0 mx-0 bg-info" href=""><h4>Brad Davis</h4></a>
      </div>
    </div>  
      <div class="d-flex col-sm-6 p-1 justify-content-center float-sm-right ">
  <!-- About is a empty link as this is the about page -->
        <div><a class="mx-1 text-secondary" href="#">About<span class="sr-only">(current)</span></a></div> 
        <div><a class="mx-1 text-secondary" href="./portfolio.html">Portfolio</a></div>
        <div><a class="mx-1 text-secondary" href="./contact.html">Contact</a></div>
       </div>
    </div>
  </header>

    <!-- Again, I used the Card class base to get a start with the formatting, and again used Picture to work with some of the responsivness -->
    <form class="container mx-1 mt-3">
        <div class="col">
            <div class="card border bg-white text-muted">
              <div class="px-3 py-3 border bg-white">
                <h3 class="card-title text-info pb-3 mb-0 border-bottom border-secondary">Portfolio</h3>
    <!-- I chose to set a fixed width to allow the screen to fill up at the largest widths, and still have a nearly full screen at xs/sm levels -->
                        <picture class="card float-left mt-3 mr-3" style="width: 16rem;">
                            <img class="img-responsive" style="max-width: 20rem;" src="https://images.pexels.com/photos/341523/pexels-photo-341523.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="Numerous Screens">
                            <div class="bg-info text-secondary px-3 py-3 text-center">
    <!-- All links should be functional and point to previous projects.  The image is related to the specific project to create this page, but I expect I'll make changes when refactoring in the future-->
                                <a class="text-white" href="https://davisbradleyj.github.io/code-refactor/">Code Refactor</a>
                            </div>
                        </picture>

                        <picture class="card float-left mt-3 mr-3" style="width: 16rem;">
                             <img class="img-responsive" style="max-width: 20rem;" src="https://images.pexels.com/photos/341523/pexels-photo-341523.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="Numerous Screens">
                             <div class="bg-info text-secondary px-3 py-3 text-center">
                               <a class="text-white" href="#">Responsiveness Portfolio</a>
                             </div>
                        </picture>
            
                        <picture class="card float-left mt-3 mr-3" style="width: 16rem;">
                            <img class="img-responsive" style="max-width: 20rem;" src="https://images.pexels.com/photos/341523/pexels-photo-341523.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500" alt="Numerous Screens">
                             <div class="bg-info text-secondary px-3 py-3 text-center">
                                <a class="text-white" href="http://davisbradleyj.github.io/Password_Generator">Password Generator</a>
                            </div>
                        </picture>


```

```css

¯\_(ツ)_/¯

```

## Acknowledgements
 Jerome Chenette, Kerwin Hy, Mahisha Manikandan, Kasey Cheng, Will Gibson, Sam Poppe, Michael Downs

## Author Links
Brad Davis
[Email](davis.bradleyj@gmail.com)
[LinkedIn](https://www.linkedin.com/in/brad-davis-7885884/)
[GitHub](https://github.com/davisbradleyj)
