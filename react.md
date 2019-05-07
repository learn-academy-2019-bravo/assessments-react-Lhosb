# React Assessments

Try your best to answer each question on your own before looking up the answer online. Once you're done writing your first answer, you can google the question and write the best answer you find.

#### 1. Here is a list of pros and cons to using the React library to build your application -- but some of them are false. Remove the false statements from the list:

- React was created to be simple, so that even people with minimal code experience could use it and create Single Page Applications (SPAs) (MAYBE????)
- React is a modern, efficient answer to complex UI applications

- React is a flexible library that plays the role of V in an MVC framework


 #### 2. What are "smart"(logic) and "dumb"(display) components? Explain the difference and also add why we bother to make the distinction between them.


 //Your Answer
Smart components actually do logic and interact with the user. Dumb components simply display an element.

 //Googled Answer
 Dumb (presentational/display) components are only responsible for presenting something to the dom. Smart components hold state to perform logic and make the app do things.


#### 3. When we use "yarn add ..." in the terminal - what is yarn doing? And what file will always be automatically updated after we add a package with yarn?


 //Your Answer
Yarn is a package manager. The yarn add ... will add the package  specified by the user (ex. "yarn add react" will add the files needed to run a react app).

 //Googled Answer
 "Yarn add" installs a package and any packages that it depends on.


#### 5. There are three mistakes in this code that would cause it to break our application. Find the mistakes and fix them:


    import React, { Component } from 'react';
                  //mistake 1
    class Recipes extends Component {
      constructor(props){
        super(props)
        this.state = {
          recipes:
            {name: 'Meatballs'},
            {name: 'Mac & Cheese'}

        }
      }

      render() {
        //miskate 2
        let { recipes } = this.state
        return (

          let recipesNames = recipes.map(function(recipe){
            return(
              <li key={recipe.name}>{recipe.name}</li>
            )
          })

          <ul>
            {recipesNames}
          </ul>
        );
      }
    }

    export default Recipes;

#### 6. Name three html input types. (NOTE: text is the default type - so it doesn't count in this case)

 //Your Answer
  Number
  Button
  Checkbox


 //Googled Answer
  <input type="button">
  <input type="checkbox">
  <input type="color">
  <input type="date">
  <input type="datetime-local">
  <input type="email">
  <input type="file">
  <input type="hidden">
  <input type="image">
  <input type="month">
  <input type="number">
  <input type="password">
  <input type="radio">
  <input type="range">
  <input type="reset">
  <input type="search">
  <input type="submit">
  <input type="tel">
  <input type="text">
  <input type="time">
  <input type="url">
  <input type="week">


 #### 7. How would you explain state to a friend who doesn't know code?

 //Your Answer
  State allows for a program to change without refreshing the entire program or changing other elements of the page. Think the like button on facebook. Clicking like changes only that items like counter.

 //Googled Answer
 "In the React sense, “state” is an object that represents the parts of the app that can change. Each component can maintain its own state, which lives in an object called this.state"


 #### 8. What is the difference between component state and props? Your answer should include a short explanation of both.


 //Your Answer
State in a react component dictates what parts of the component are interactive with the user. State is only managed inside the component. Props, short for properties, are a way to pass variables into a component.

 //Googled Answer
The main difference between state and props is scope. A component state is local and cannot be accessed outside of its component. Props are a way to pass identifiers into components in order to make them unique.

#### 9. Write a paragraph or so about your experience with building tic-tac-toe. Some topics to start with might be: things you learned about yourself, concepts from React that stood out to you, something about pair programming (if you paired), or the experience of building something in code from scratch.
