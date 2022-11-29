[Home](../README.md)

# Class 2

## Express, NPM, TDD, CI/CD

### NodeJS and Express [Express/Node Introduction - MDN](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)

1. Middleware is any function that is used by a server to perform some action based on an API call. It can run before or after the server request is handled.

2. Express is the most popular Node web framework. From MDN, It allows us to: 

    - Write handlers for requests with different HTTP verbs at different URL paths (routes).
    - Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
    - Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.
    - Add additional request processing "middleware" at any point within the request handling pipeline.

3. Express is unopinionated, meaning it does not prescribe specific ways to handle cases, but allows for the use of a variety of solutions and tools for whatever problem in the form of middleware.

4. A module is a unit of code. It exists as a standalone file or directory that can be imported into another codebase. Benefits of modularity are ease of testing, future-proofing, reuseability, and more.

### NPM [NPM - npmjs.com](https://docs.npmjs.com/about-npm)

1. I am runing npm v8.15.0

2. To install 'jshint', I would run `npm install jshint` (or `npm i jshint`)

### TDD [TDD - Agile Alliance](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))

1. Tests are important because they give us an auomated view of the health of our app as we develop and make changes. They are an objective and consistent wayfor us to see if our code and its subcomponents are running the way we expect them to.

2. Expected benefits of testing are:

    - a reduction in defect rates
    - a reduction in effort in later project phases, at the expense of greater effort in beginning phases
    - potentially improved design qualities

3. Some pitfalls include:

    - Individual:

      - Not running tests frequently
      - Writing too many tests at once
      - Not testing at a fine-grained level
      - writing overly trivial tests
      - writing tests fro trivial code

    - Team:

      - partial adoption of TDD across the team
      - poor maintenance of tests

### CI/CD [CI/CD - Github Training Guides](https://www.youtube.com/watch?v=nI5VdsVl0FM)

1. Continous Integration offers some key benefits:

    - Ensures everyone's changes are integrated
    - Catches bugs
    - Reduces merge conflicts

2. 
