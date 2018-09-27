# Notes in Learning VUE

​                                          WEI Xiao-Miao 516015910018

## 1. Intro of Vue

### 1.1 What is Vue

> Vue (pronounced /vjuː/, like **view**) is a **progressive framework** for building user interfaces. Unlike other monolithic frameworks, Vue is designed from the ground up to be incrementally adoptable. The core library is focused on the view layer only, and is easy to pick up and integrate with other libraries or existing projects. On the other hand, Vue is also perfectly capable of powering sophisticated Single-Page Applications when used in combination with modern tooling and supporting.
>
> ​                                                                *from*   *vuejs.org*

To briefly conclude the intro above Vue.js is

- **A framework (or lib) of javascript to build an interactive web page;**
- **A group of web page widgets bound with datas and useful APIs.**

### 1.2 Features of Vue

- Concise: it simplifies the front-end project into HTML template + datas + Vue instance.
- Data drive: it can trace expression in template and calculates by the shared data.
- Modularity: coupling and decoupling modules to build the page.
- Lightweight: it weights only 24kb and has no dependency on other frameworks.
- Swift: precisely realize the update of DOM through asynchronism.
- Progressive: it can be partly or totally uesed in the whole script of a website.

### 1.3 Conception of Vue

The core concepton of Vue is its **reusable components**.

In the perspective of Vue, the front-end page could be seen as an **assembly of a group of vue instances**, and each one contains its own HTML, CSS and Javascript. All those vue components render the anywhere in the piece of webpage.

![componentsStruct](./images/componentsStruct.jpg)

Vue components also handle with datas and reactions. which is called **data bound**. To realize this, vue components store datas as members and react with input and display datas in the page by the same lable in HTML(''id'') and script(''el'').

## 2. Coding in Vue

### 2.1 Installation

1. Direct <script> Include

   Simply vue.js and include with a script tag when develop front-end page or small scale application. Vue will be registered as a global variable. Or link to CDN in HTML like:

   ```html
   <script src="https://cdn.jsdelivr.net/npm/vue@2.5.17/dist/vue.js">
   </script>
   ```

    

2. NPM install

   When building large scale applications with Vue, npm installation pairs nicely with module bundlers such as Webpack or Browserify. Vue also provides accompanying tools for authoring Single File Components.

   ```
   $ npm install vue
   ```

### 2.2 An vue instance

The core conception( as mentioned in 1.3 ) is to use vue instance to render data in to components on the webpage. 

In HTML file, component bounds with vue instance by id and show datas in {{}}. Like:

```html
<div id="app">
  {{ message }}
</div>
```

Coherently, in script, an vue instance is created through vue constructor. Like:

```javascript
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue!'
  }
})
```

What is show on the webpage is as follow:

> Hello Vue!

### 2.3 Lifetime of an Vue instance

![lifecycle](./images/lifecycle.png)

## 3. Inner realization of Vue 

## 4. Tools in Vue

## 5. Largescale develop in Vue

