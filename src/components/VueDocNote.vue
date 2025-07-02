<template>
  <div>
    <h1>Creating an Application</h1>
    <div>
      <p>Create a new application instance with the createApp() function.</p>
      <p>
        <li>The passing object in createApp() function is a Root-Component</li>
        <li>import root component and imple</li>
        <li>An application instance won't be run anything until it's Mound() method is called.</li>
        <li>use multiple components in the root component for a better understanding.</li>
      </p>
    </div>
    <div>
      <p>Template syntax</p>
      <p>
        <li>Text Interpolation.</li>
        <li>Directives and Mustaches.</li>
        <li>v-bind for html attributes.</li>
        <li>Boolean Attributes</li>
      </p>
    </div>
    <div>
      <p>Reactivity Fundamentals</p>
      <p>
        <li>To Declare reactive state we use ref() Function.</li>
        <li>ref() value is accessible by using the .value</li>
        <li>In template the ref() value will get automatically Uncovered.</li>
        <li>reactive() API</li>
      </p>
    </div>
    <div>
      <p>Computed Properties</p>
      <p>
        <li>
          To make easy to make any other functions with the data inside a reactive() functions, we
          can use the computed to make it clean the Template.
        </li>
        <li></li>
      </p>
    </div>
    <div>
      <p>Class and Style Bindings</p>
      <p>
        <li>we can have the class names with objects.</li>
      </p>
    </div>
    <div>
      <p>Components Basics</p>
      <p>
        <li>Can import components and use it</li>
        <li>We can define props.</li>
        <li>In component we can define the props for it.</li>
        <li>
          so when we call the component we can give the props and access it in the parent component
          too.
        </li>
        <li>Listening to events.</li>
        <li>Use Custom Slot.</li>
        <li>custom slot to do an alert box</li>
        <li>Use the '<slot />'</li>
      </p>
    </div>
    <div>
      <p>Lifecylcle Hooks</p>
      <p>----------------</p>
      <p>
        <li>Registering Lifecylcle hooks</li>
        <li>Hooks for eg: onMounted , onUpdated, and onUnMounted.</li>
        <li>
          mounted: Called after the component is mounted to the DOM. DOM elements are now
          accessible.
        </li>
        <li>unMounted: Called after the component is unmounted from the DOM.</li>
        <li>Lifecylcle Diagram</li>
      </p>
    </div>
    <div>
      <p>TypeScript with Composition API</p>
      <p>-------------------------------</p>
      <p>Overview ofTypeScript.</p>
      <p>
        <li>Typing Component Props</li>
        <li>runtime declaration - eg: definePorps()</li>
        <li>definePorps with generic type argument - Type-based declaration.</li>
        <li></li>
      </p>
    </div>
  </div>
  <div>
    <div>
      <p>TypeScript with Composition API</p>
      <p>-------------------------------</p>
      <p>Overview ofTypeScript.</p>
      <p>
        <li>Typing Component Props</li>
        <li>runtime declaration - eg: definePorps()</li>
        <li>definePorps with generic type argument - Type-based declaration.</li>
        <li></li>
      </p>
    </div>
    <div>
      <p>Git merge</p>
      <p>Resolve the Conflict error.</p>
      <p>
        <li>from the main branch</li>
        <li>:git pull origin main</li>
        <li>Go to the new branch</li>
        <li>:git merge main</li>
        <li>:git add .</li>
        <li>:git commit -m ""</li>
        <li>:git push origin branch/name</li>
      </p>
    </div>
    <div>
      <p>after merging</p>
      <p>
        <li>checkout to main branch.</li>
        <li>:git checkout main</li>
        <li>Then by git pull take all the changes to the local repo.</li>
        <li>:git pull</li>
      </p>
    </div>
    <div>
      <p>For changes in other branches</p>
      <p>
        <li>In the parent branch</li>
        <li>:git pull origin branch-name</li>
        <li>got to the branch where u need the other branch datas</li>
        <li>:git merge parent-branch-name</li>
      </p>
    </div>
  </div>
</template>

<script setup></script>
