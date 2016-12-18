<template>
    <div id="resume" class='project-container'>
      <header>
        <button>Resume</button>
      </header>
      <main>
        <header>
          <h3>Phone: <a href='tel:8179955467'>(773)668-6100</a></h3>
          <h3>Email: <a href='mailto:paigeinteractive@gmail.com?subject=Hey,%20I%20saw%20your%20website...'>PaigeInteractive@gmail.com</a></h3>
          <h3>Github: <a href='http://github.com/paige-keenan' target='_blank'>@paige-keenan</a></h3>
        </header>

        <section>
          <article>
          <h2>Experience</h2>
            <section>
              <h3>Wyzant</h3>
              <h4>Chicago, IL &mdash; <a href='http://www.wyzant.com/' target='_blank'>Learn More</a></h4>
              <h5>Front End Developer: August 2016 - Present</h5>
              <p>I joined the agile marketing development team of Wyzant where we facilitated a full site rebrand, implement site enhancements, and complete all maintenace support. In the time I've been here, I've created a Gulp task runner to make the front end coding process more effecient, worked within C#, GoLang, Gulp, and the typical front end languages, and continue to work on and fulfill all deliverable site enhancements every sprint duration.</p>
            </section>

            <section>
              <h3>Razorfish</h3>
              <h4>Atlanta, GA &mdash; <a href='http://www.razorfish.com/' target='_blank'>Learn More</a></h4>
              <h5>Presentation Layer Engineer: January 2016 - August 2016</h5>
              <p>In this role, I have provided maintenance work on Bridgestone Tire's website, been a core member of the development team that launched Firestone Tire's latest rendition of their website, and joined the team of a large banking website where my role includes maintenance and configuring unit tests to better expedite and ensure quality code.</p>
            </section>

            <section>
              <h3>Razorfish</h3>
              <h4>Atlanta, GA &mdash; <a href='http://www.razorfish.com/' target='_blank'>Learn More</a></h4>
              <h5>Associate Presentation Layer Engineer: September 2014 - January 2016</h5>
              <p>As an associate level developer, I worked on the maintenance and measurements tracks of Bridgestone Tire's and Firestone Tire's websites, assisted in the complete redesign and infrastructure of Bridgestone Tire's latest rendition of their website, and worked on seasonal promotions under the Bridgestone Tire / Firestone Tire umbrella.</p>
            </section>

            <section>
              <h3>100 Girls of Code</h3>
              <h4>Atlanta, GA &mdash; <a href='http://www.100girlsofcode.com/' target='_blank'>Learn More</a></h4>
              <h5>Atlanta Chapter Co-Founder: April 2015 - January 2016</h5>
              <p>My role included creation of lesson plans for girls aged 8 through 18 - lessons varying by age group, scouting of locations to host monthly web development learning camps, teaching an all female group of code-savy instructurs the monthly lesson plan, and being the lead instructor of each camp we hosted. Lesson plans taught included: HTML / CSS, basic computer science fundamentals, critical thinking excercises, Unity game development, Scratch software, CSS animations, intro to Python, and more.</p>
            </section>

            <section>
              <h3>JENI'S SPLENDID ICE CREAMS</h3>
              <h4>Atlanta, GA &mdash; <a href='https://jenis.com/' target='_blank'>Learn More</a></h4>
              <h5>Ice Cream Ambassador: September 2013 - September 2014</h5>
              <p>I scooped ice cream and taught people the importance of quality ingredients in order to make superior ice creams to endless lines of customers and absolutely loved it. You can ask me anything about ice cream. I know too much about ice cream.</p>
            </section>
          </article>

          <article>
            <h2>Education</h2>
            <section>
              <h3>THE CREATIVE CIRCUS</h3>
              <h4>Atlanta, GA &mdash; <a href='http://creativecircus.edu/' target='_blank'>Learn More</a></h4>
              <h5>Interactive Development Student: October 2013 - September 2014</h5>
              <p>I learned the core concepts of front end development at an advertising school focused on both creating great designers and sought after developers. While at school, I learned basic front end, the Adobe Suite, frameworks including Angular JS, Vanilla JavaScript, Unity game development, and multiple animation libraries.</p>
            </section>
          </article>

          <article id="skills">
            <h2>Skills</h2>
            <h3>Languages</h3>
            <section>
              <ul>
                <li>HTML5 | Jade | Haml</li>
                <li>CSS3 | SCSS | SASS | Less</li>
                <li>JavaScript | CoffeeScript</li>
                <li>React JS</li>
              </ul>
            </section>

            <section>
              <h3>frameworks</h3>
              <ul>
                <li>Vue JS</li>
                <li>Angular JS</li>
                <li>Backbone</li>
              </ul>
            </section>

            <section>
              <h3>CMS Expertise</h3>
              <ul>
                <li>Adobe Experience Manager</li>
                <li>Siteleaf (with Jeykll integration)</li>
                <li>Wordpress</li>
                <li>Shopify</li>
                <li>Orchard</li>
                <li>Squarespace</li>
                <li>Unbounce</li>
              </ul>
            </section>

            <section>
              <h3>Tools</h3>
              <ul>
                <li>Atom</li>
                <li>Git | SourceTree</li>
                <li>Terminal</li>
                <li>Grunt | Gulp</li>
                <li>Node JS</li>
                <li>Underscore</li>
                <li>Handlebars</li>
                <li>Creative Suite</li>
                <li>JIRA | Trello</li>
              </ul>
            </section>
          </article>
      </main>
  </div>
</template>
<style lang="scss">
#resume {
  main {
      padding: 2em 1em;
  }
  header {
      padding-bottom: 15px;
      h3 {
          font-family: "Open Sans", sans-serif;
          text-transform: uppercase;
          font-size: 12px;
          letter-spacing: 1px;
          text-align: left;
          font-weight: 400;
      }
      a {
          color: #000;
          text-decoration: underline;
      }
  }
  h2 {
      font-family: "Open Sans", sans-serif;
      text-transform: uppercase;
      font-size: 30px;
      letter-spacing: 1px;
      text-align: center;
      margin-bottom: 0;
  }
  section {
      position: relative;
      h3 {
          font-family: "Open Sans", sans-serif;
          text-transform: uppercase;
          letter-spacing: 1px;
          font-weight: 400;
          font-size: 15px;
          margin: 0;
          padding-top: 30px;
      }
      h4 {
          font-family: 'Gentium Basic', serif;
          margin: 0;
          letter-spacing: 1px;
          margin: 5px 0;
          a {
              text-decoration: underline;
              color: #000;
          }
      }
      h5 {
          font-family: 'Gentium Basic', serif;
          font-size: 12px;
          letter-spacing: 1px;
          color: #383838;
          margin: 0;
          line-height: 15px;
      }
      p {
          margin: 1em 0;
          line-height: 24px;
          font-size: 12px;
          padding-bottom: 30px;
      }
      &:after {
          content: '';
          position: absolute;
          bottom: 0;
          left: 0;
          right: 0;
          margin: 0 auto;
          width: 20px;
          height: 4px;
          background: #000;
      }
      &:last-of-type:after {
          display: none;
      }
      li {
          font-family: "Open Sans", sans-serif;
          padding: 0 0 .5em;
          font-size: 12px;
      }
  }
  #skills section:after {
      display: none;
  }
}
</style>
