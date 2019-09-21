# 100 Days of Code - Log

## Day 1: March 17, 2019
**Today's Progress:**
1. JavaScript (60mins)
2. GatsbyJS (100mins)

**Thoughts:**
I am restarting ES6 for Everyone. It's good to go through these courses again as I can tell I comprehend more than I did last time. I also see functions available in JS that are available in other languages and it makes me think about opportunities I have in other projects to use them.
I later finished the GatsbyJS tutorial available on the Gatsby website. I worked with GraphQL a little bit more and with the final steps before taking a site live such as Auditing with Lighthouse. I found the manifest and related steps to be interesting.

**Today's Links:**
1. [ES6 for Everyone](https://es6.io/)
2. [GatsbyJS Tutorial](https://www.gatsbyjs.org/tutorial/part-eight/)

## Day 1: August 26, 2019
**Today's Progress:**
1. WordPress (60mins)

**Thoughts:**
Even though I've writting a couple of plugins for production, I wanted to go through a more structured process of creating a plugin. I found this series of articles on [Torque](https://torquemag.io/) that are good resource. Tonight I'll probably go through the process again and create a new plugin for the website.

**Today's Links:**
1. [BUILDING A WORDPRESS PLUGIN: FIRST STEPS AND SETTING THE SCENE](https://torquemag.io/2016/08/building-a-wordpress-plugin-part-1-first-steps-and-setting-the-scene/)
2. [BUILDING A WORDPRESS PLUGIN PART 2: GETTING OFF TO A SOLID START](https://torquemag.io/2016/08/building-wordpress-plugin/)
3. [BUILDING A WORDPRESS PLUGIN PART 3: SETTING UP A CUSTOM CONTENT TYPE](https://torquemag.io/2016/09/building-a-wordpress-plugin-part-3-setting-up-a-custom-content-type/)
4. [BUILDING A WORDPRESS PLUGIN PART 4: LOOKING AT DISPLAYING CONTENT VIA SHORTCODES](https://torquemag.io/2016/09/building-a-wordpress-plugin-part-4-looking-at-displaying-content-via-shortcodes/)
5. [BUILDING A WORDPRESS PLUGIN PART 5: FINISHING OFF OUR SETTINGS](https://torquemag.io/2016/09/building-a-wordpress-plugin-part-five/)
6. [BUILDING A WORDPRESS PLUGIN PART 6: FURTHER OPTIONS AND FINAL THOUGHTS](https://torquemag.io/2016/09/building-wordpress-plugin-part-6/)

## Day 1: August 31, 2019
**Today's Progress:**
1. React (70mins)

**Thoughts:**
I'm redoing a lesson on React because I've been having trouble remembering the exact syntax for ReactDOM.render(). I know the basic layout but I keep on forgetting the exact way to enter the first argument. I studied `this.props`. Glad I went through it a 2nd time, definitely feel like I have a better grasp. Later, I'll go through `this.state`.
`ReactDOM.render(<ComponentName />, document.getElementById('app'));`

**Today's Links:**
1. [React - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)

## Day 2: September 1, 2019
**Today's Progress:**
1. React (70mins)

###Thoughts:
Today I went through two lessons I had done before. These focused on `state` and `props`.
**State**. A React component can access dynamic information in two ways: `props` and `state`. Unlike `props`, a component's `state` is not passed in from the outside. A component decides it's own `state`. To make a component have `state`, give the component a `state` property.
```
class Example extends React.Component {
  constructor(props) {
    super(props);
    this.state = { mood: 'decent' };
  }

  render() {
    return <div></div>;
  }
}

<Example />
```
`this.state` should be equal to an object - like above.
**React components *always* have to call `super` in their constructors to be set up properly**.
A Component can read and *change* it's own state. A component changes it's state by calling the function `this.setState()`.
The most common way to call `this.setState()` is to call a custom function that wraps a `this.setState()` call.
```
import React from 'react';
import ReactDOM from 'react-dom'

const green = '#39D1B4';
const yellow = '#FFD712';

class Toggle extends React.Component {
  constructor(props) {
  	super(props);
    this.state = { color: green };
    this.changeColor = this.changeColor.bind(this);
  }
  
  changeColor() {
    const newColor = this.state.color == green ? yellow : green;
    this.setState({color: newColor});
  }
  
  render() {
    return (
      <div style={{background: this.state.color}}>
        <h1>
          Change my color
        </h1>
        <button onClick={this.changeColor}>
        	Change color
        </button>
      </div>
    );
  }
}
```

###Today's Links:
1. [React - Rendering Elements](https://reactjs.org/docs/rendering-elements.html)

## Day 3: September 2, 2019
**Today's Progress:**
1. Gatsby (110mins)

**Thoughts:**
Started the Gatsby tutorial again. Part zero consisted of setting up the development environment and learning basic commands such as `gatsby develop`.
When creating a new gatsby site, use the following command structure to create a new site based on any existing Gatsby starter:
```
gatsby new [SITE_DIRECTORY_NAME] [URL_OF_STARTER_GITHUB_REPO]
```
A "component" could be defined as a building block for your site. A self-contained piece of code that describes a section of user interface.

**Today's Links:**
1. [Gatsby - Set Up Your Development Environment](https://www.gatsbyjs.org/tutorial/part-zero/)
2. [Gatsby - Get to know Gatsby building blocks](https://www.gatsbyjs.org/tutorial/part-one/)

## Day 4: September 3, 2019
**Today's Progress:**
1. WordPress (70mins)

**Thoughts:**
Today I spent some time going through a tutorial I have gone through once before. This is about building a WordPress theme from scratch. The biggest snippet I gathered this time around is the workflow to creating the theme. The instructor recommended a seperate environment to create the static pages for the theme. This is brilliant. This saves all the time from creating the dev environment on multiple machines and instead gets you coding quick.

**Today's Links:**
1. [WordPress Theme Development](https://www.udemy.com/bootstrap-to-wordpress)

## Day 5: September 4, 2019
**Today's Progress:**
1. WordPress (60mins)

**Thoughts:**
Today's lessons were mostly about styling. Nothing really new encountered here.

**Today's Links:**
1. [WordPress Theme Development](https://www.udemy.com/bootstrap-to-wordpress)

## Day 6: September 6, 2019
**Today's Progress:**
1. Gatsby (30mins)
2. React (20mins)

**Thoughts:**
I worked on Styling in Gatsby and learned about CSS Modules. I felt mostly comfortable with the syntax of everything. This article didn't go into CSS-in-JS but there were a few other articles mentioned for more information.
I also went through a short tutorial on Codecademy regaring stateless and stateful components. I felt mostly comfortable with that. I'll have to go through more lessons to really 'put it together' though.

**Today's Links:**
1. [Introduction to Styling in Gatsby](https://www.gatsbyjs.org/tutorial/part-two/)

## Day 6: September 10, 2019
**Today's Progress:**
1. WordPress (60mins)
2. Gatsby (40mins)

**Thoughts:**
Watched more of the WordPress theme development course. Most of the material was pretty basic. The one lecture that included a brief discussion on the usage of sprites was probably the best piece of information for me.
The Gatsby tutorial focused on utilizing plugins in Gatsby and creating and using components. I also went off-tutorial and created a table component which I used on one of the pages.

**Today's Links:**
1. [WordPress Theme Development](https://www.udemy.com/bootstrap-to-wordpress)
2. [Creating nested layout components](https://www.gatsbyjs.org/tutorial/part-three/)

## Day 7: September 12, 2019
**Today's Progress:**
1. AJAX/XHR (50mins)
2. WordPress (30mins)
3. React (40mins)

**Thoughts:**
I spent time trying to get an XHR request to work with Salesforce Marketing Cloud but was hampered by an error stating: `Access to XMLHttpRequest at 'https://domain.net/subscribe.aspx?lid=1267' from origin 'http://playground.test:3000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource.` I reached out to Marketing Cloud regarding the proper format required.
I spent some time watching the WordPress Theme Development series and it was mostly review of layout (CSS).

**Today's Links:**
1. [WordPress Theme Development](https://www.udemy.com/bootstrap-to-wordpress)

## Day 8: September 13, 2019
**Today's Progress:**
1. Flywheel (180mins)

**Thoughts:**
Worked on getting the development environment for phoenixstartupweek set up. We also worked on getting version control on github set up, but instead will use gitlab due to the permissions management.

**Today's Links:**
1. [Local by Flywheel](https://localbyflywheel.com/)

## Day 9: September 14, 2019
**Today's Progress:**
1. Gulp 4 Boilerplate (215mins)

**Thoughts:**
Today, I created a Gulp 4 boilerplate and project scaffold from scratch. The task syntax is a little different in Gulp 4. I used several resources to set up the functionality but it did take me some time to figure out adding BrowserSync functionality. This project also fixes some of the issues I've had with other environments such as auto-reloading when image files are added to the image directory.

**Today's Links:**
1. [Using Gulp 4 in your workflow for Sass and JS files](https://coder-coder.com/gulp-4-walk-through/)

## Day 10: September 17, 2019
**Today's Progress:**
1. WordPress Theme Development (65mins)

**Thoughts:**
Working through the theme develpment course. These lessons focused on laying out ui and css.

**Today's Links:**
1. [Using Gulp 4 in your workflow for Sass and JS files](https://coder-coder.com/gulp-4-walk-through/)

**Today's Links:**
1. [Using Gulp 4 in your workflow for Sass and JS files](https://coder-coder.com/gulp-4-walk-through/)

## Day 11: September 18, 2019
**Today's Progress:**
1. Gatsby (65mins)

**Thoughts:**
In part 4 of the tutorial wrote a graphql page query to query the title for my about page. Then, I wrote a `StaticQuery` which allows non-page components to retreive data via GraphQL queries.
In part 5 I was introduced to GraphiQL and saw how I could use it to visually see site data. I then used a source plugin `(source plugins fetch data from their source... The WordPress plugin knows how to fetch data from the WordPress API)` to query data.

**Today's Links:**
1. [Data in Gatsby](https://www.gatsbyjs.org/tutorial/part-four/)
1. [Source plugins and rendering queried data](https://www.gatsbyjs.org/tutorial/part-five/)
2. [How to GraphQL](https://www.howtographql.com/)

## Day 12: September 19, 2019
**Today's Progress:**
1. Gatsby/WordPress (180mins)

**Thoughts:**
Worked with another developer on a non-profit project. We're using a WP backend with a Gatsby frontend. We're still in the planning and setup phase. I helped him get his `Gulp 4` dev environment set up his *Windows* computer using the boiler plate I worked on last week. We also worked on adding a new custom post type using ACF- this will be our prototype for the Gatsby front end. We added a few tasks in Asana and then called it a night.

**Today's Links:**
1. [Data in Gatsby](https://www.gatsbyjs.org/tutorial/part-four/)
2. [Source plugins and rendering queried data](https://www.gatsbyjs.org/tutorial/part-five/)
3. [How to GraphQL](https://www.howtographql.com/)

## Day 13: September 20, 2019
**Today's Progress:**
1. GitLab (30mins)
2. MySQL (180mins)

**Thoughts:**
Moved a repository from GitHub to GitLab. Currently, working within a team, the permissions seem to be more flexible in the free tier on GitLab. At first the permissions seemed confusing but I just needed to create a new group.
I worked on queries in MySQL on the WordPress database. I learned a little more about how data is stored- especially Metadata. I also installed Sequel Pro on my work computer. I wasn't sure if I needed it anymore and I found it was more convenient to write queries there instead of in the command line.
I also saw a cool code snippet in Frontend Focus to give a visual indicator if an image doesn't have an alt attribute:
```
img:not([alt]) {
  filter: grayscale(100%);
}
```

**Today's Links:**
1. [Phoenix Startup Week](https://phxstartupweek.com)
2. [GitLab - Organization Account](https://forum.gitlab.com/t/organisation-account/14026/5)
3. [Frontend Focus](https://frontendfoc.us/issues/409)
