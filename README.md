# Work Day Schedule
## Website Description

This Website allows the user to create and save a schedule to local storage

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

What things you need to install the software and how to install them

```
Github and Gitlab accounts
GitBash or Terminal
```

### Installing

A step by step series of examples that tell you how to get a development env running

```
Clone the code to your terminal
Pull from the repository
View on Visual Studio Code
```

## Built With

* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [JavaScript](https://www.javascript.com/)
* [jQuery](https://jquery.com/)

## Deployed Link

* [See Live Site](https://hudsonmbarnes.github.io/schedule/)

## What I did

Using the templates given to me, I coded a way for the user to use local storage to store information on a schedule. 

## Code Snippet

This part of the code is the function displaying the date and time. It also displays a save button that saves the users imput to local storage.

```
$(document).start(function () {
    //display current day & time
    $("#currentDay").text(moment().format("MMMM Do YYYY, h:mm:ss a"));

    $(".saveBtn").on("click", function () {
        console.log(this);
        var text = $(this).siblings(".description").val();
        var time = $(this).parent().attr("id");

        //set items in local storage.
        localStorage.setItem(time, text);
    })

```

## Editors

* **Hudson Barnes**
- [Link to Github](https://github.com/hudsonmbarnes)
- [Link to LinkedIn](https://www.linkedin.com/in/hudson-barnes-398483151/) 


## Authors

* **Hudson Barnes** 


## Acknowledgments

* W3schools.com
* stackoverflow.com
* google.com
* github.com