# Front End Profile Component
This hustle test is for a __front-end developer__. This is a front end exercise
for a component we need to implement across a number of our applications; `map`,
`search`, `messenger` and `UI`.

#### Problem to Solve
The task is to create a reusable component in either `Vue.js`, `React` or
`AngularJs` that provides a web element/component that manages state. When the component
is deployed in a UI environment, the component needs to be aware of the visitors
`auth state`, via the Firebase Auth SDK. It needs to show a different HTML content
depending on this state. When the user is `unknown` it needs to show a 'Get Started'
button that when clicked takes the user to either a registration page, or open
a registration/login modal. When the user is `known` (already logged-in) the component
needs to open a dropdown element that shows them options: My Account, List of Message
etc.

This `profile` component will then be used on the following web components. Each of
these currently have localized code for these actions. Long term we want to pull
all profile like activity out of the codebase and have it reside in this component.

Here are some mockups and screenshots.

- [https://map.meenta.io](https://map.meenta.io) - Simple mockup - [Map with Profile](/assets/Map-Profile-Example.png)
- [https://meenta.io/search](https://meenta.io/search) - Simple mockup - [Search with Profile](/assets/Search-Profile-Example.png)
- [https://meenta.io/messenger](https://meenta.io/messenger)

### Resources
- [Balsamiq Mockup](/assets/General-Mockup.png)
- [Gmail Header Example](/assets/Google-Profile.png)

#### Deliverables
The objective of this test is to demonstrate an understanding of re-usable web
components that can be used in different context and environments. This assumes
that the component will load it requirements in a single bundle and can be called
from any UI. And will include usage documentation that tells other developers
how to implement.

- Code for UI component.
- Update the Bootstrap Index.html to show the code.
- Needs to be able to show both states: logged in and visitor.
- Optional - Add in `Gulp` or `Webpack` config/tasks to build bundle to `/dist` folder.

AngularJs usage example:

    1. Reference the bundle in the header:

       <script src="https://assets.meenta.io/profile/bundle.js"></script>

    2. Bootstrap using the following:

       <script>
         angular.element(document).ready(function () {
           angular.bootstrap(document, ['meenta.profile', ...]);
         });
       </script>

    3. Add the following to the UI.

       <div title="Welcome" meenta-profile></div>
       or
       <div title="Start" meenta-profile></div>

#### Note
Loading two or more components each include the same framework or libraries can
cause a problem, so the base framework (ng, react, vue.js) should not be included
in the `bundle.js`.
