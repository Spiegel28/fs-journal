# Single Page Applications with Vue
01. What is the entrypoint of an application?

  > Main.js

02. What is the difference between a vue `component` and `page`?

  > a page is automatically included in the router 

03. What is ***Component-Based Architecture***?

  > Component-Based Architecture is a software design approach where a system is decomposed into individual, self-contained, and reusable components. 

04. What are the three tags that make up a Vue component?

  > template style script 

05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > 
 "lifecycle hooks" are special methods provided by the Vue instance that allow you to execute code at specific stages of a component's lifecycle. These hooks give you the ability to perform actions when certain events occur during the lifespan of a component, such as before it is mounted, updated, or destroyed.

06. Which component in Vue does the vue-router use to mount pages onto?

  >  the vue-router library uses the <router-view> component to mount pages onto.

07. What is the difference between the `AppState` and the state object within a component?

  > AppState refers to the global state of the entire application managed by state management libraries like Vuex or Redux, while the state object within a component refers to the local state specific to that particular component, managed internally by the component itself

08. What is the responsibility of `Services` in our Vue projects?

  > modules or classes responsible for handling communication with external APIs, managing data fetching and manipulation, and encapsulating business logic that is not directly related to UI components. 

09. What are ***props*** and how are they used? Provide an example

  > "props" (short for properties) are a way to pass data from a parent component to a child component. Props allow you to create reusable components that can accept data from their parent components, making your code more modular and maintainable.



10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > watch()
