# Front End Profile Component
This hustle test a front end exercise for a component we need to implement across
a number of our applications; map, search, messenger and UI.

#### Problem to Solve
The task is to setup create an reusable component in either `Vue.js`, `React` or
`AngularJs` that provides a UI component that manages state. When the component
is deployed in a UI environment, the component needs to be aware of the visitors
`auth state`, via the Firebase Auth SDK. It needs to show a different HTML content
depending on this state. When the user is unknown it needs to show a 'get Started'
button that when clicked takes the user to either a registration page, or open
a registration/login modal. When the user is known (already loggedin) the component
needs to open a dropdown element that shows them options: My Account, List of Message
etc.

This `profile` component will then be used on the following web components. Each of
these currently have localized code for these actions. Long term we want to pull
all profile like activity out of the codebase and have it reside in this component.

Here are some mockups and screenshots.

- [Basic Mockup](/assets/General-Mockup.png)
- [Google Example](/assets/Google-Profile.png)
- [Map](https://map.meenta.io) - [Map with Profile](assets/Map-Profile-Example.png)
- [Search](https://meenta.io/search) - [Search with Profile](assets/Search-Profile-Example.png)
- [Messenger](https://meenta.io/messenger)


#### Deliverables
The objective of this test is to demonstrate an understanding of resuable web
components that can be used in different context. This assumes that the component
will load it requirements in a single bundle and can be called from any UI. And
will include usage documentation that tells other developers how to implement.

example:
    Ng: <div title="Welcome" meenta-profile></div>

- Code for UI component.
- Update the Bootstrap Index.html to show the code.
- Needs to be able to show both states: logged in and visitor.

#### Note
Loading two or more components each include the same framework or libraries can
cause a problem, so the base framework (ng, react, vue.js) should not be included
in the `bundle.js`.
