# 05 Third-Party APIs: Work Day Scheduler

Create a simple calendar application that allows the user to save events for each hour of the day. This app will run in the browser and feature dynamically updated HTML and CSS powered by jQuery.

You'll need to use the [Moment.js](https://momentjs.com/) library to work with date and time. Be sure to read the documentation carefully and concentrate on using Moment.js in the browser.

## User Story

```
AS AN employee with a busy schedule
I WANT to add important events to a daily planner
SO THAT I can manage my time effectively
```

## Acceptance Criteria

```
GIVEN I am using a daily planner to create a schedule
WHEN I open the planner
THEN the current day is displayed at the top of the calendar
WHEN I scroll down
THEN I am presented with timeblocks for standard business hours
WHEN I view the timeblocks for that day
THEN each timeblock is color coded to indicate whether it is in the past, present, or future
WHEN I click into a timeblock
THEN I can enter an event
WHEN I click the save button for that timeblock
THEN the text for that event is saved in local storage
WHEN I refresh the page
THEN the saved events persist
```

The following animation demonstrates the application functionality:

![day planner demo](./Assets/05-third-party-apis-homework-demo.gif)

## Review

You are required to submit the following for review:

* The URL of the deployed application.

* The URL of the GitHub repository. Give the repository a unique name and include a README describing the project.

- - -
© 2019 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.



Work Day Scheduler

Variable - Find the current day 
Variable - find the current time

function - generate eight rows with the hour blocks 9am-5pm
for each row, include
    a box for the time
    a free text field for the task
    a button to save the input
send the input in the field to local storage

let taskList = [];

function saveTask()
    preventDefault();
        let task = {
            time: document.getElementbyID("9am").value,
            activity = document.getElementbyID("9am").value
        }
taskList.push(task);
localStorage.setItem("MyTaskList", tasklist);

    var 9amTask = document.getElementbyID("9am").value;
    var 10amTask = document.getElementbyID("10am").value;
    var 11amTask = document.getElementbyID("11am").value;
    var 12pmTask = document.getElementbyID("12pm").value;
    var 1pmTask = document.getElementbyID("1pm").value;
    var 2pmTask = document.getElementbyID("2pm").value;
    var 3pmTask = document.getElementbyID("3pm").value;
    var 4pmTask = document.getElementbyID("4pm").value;

<input type="text" name="" id="9am">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="10am">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="11am">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="12pm">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="1pm">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="2pm">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="3pm">
<button onclick=saveTask()>Save Task</button>
<input type="text" name="" id="4pm">
<button onclick=saveTask()>Save Task</button>

    function saveTask()
      var nineamTask = document.getElementbyID("9am").value;
      var tenamTask = document.getElementbyID("10am").value;
      var elevenamTask = document.getElementbyID("11am").value;
      var twelvepmTask = document.getElementbyID("12pm").value;
      var onepmTask = document.getElementbyID("1pm").value;
      var twopmTask = document.getElementbyID("2pm").value;
      var threepmTask = document.getElementbyID("3pm").value;
      var fourpmTask = document.getElementbyID("4pm").value;



      <row>
  <p class = "timeBlock">10am</p>
<input type="text" name="" id="10am">
<button class=saveBtn>Save Task</button>
</row>
<row>
  <p class = "timeBlock">11am</p>
<input type="text" name="" id="11am">
<button class=saveBtn>S>Save Task</button>
</row>
<row>
  <p class = "timeBlock">12pm</p>
<input type="text" name="" id="12pm">
<button class=saveBtn>S>Save Task</button>
</row>
<row>
  <p class = "timeBlock">1pm</p>
<input type="text" name="" id="1pm">
<button class=saveBtn>S>Save Task</button>
</row>
<row>
  <p class = "timeBlock">2pm</p>
<input type="text" name="" id="2pm">
<button class=saveBtn>S>Save Task</button>
</row>
<row>
  <p class = "timeBlock">3pm</p>
<input type="text" name="" id="3pm">
<button class=saveBtn>S>Save Task</button>
</row>
<p class = "timeBlock">4pm</p>
<row><input type="text" name="" id="4pm">
<button class=saveBtn>S>Save Task</button>
</row>



$(".saveBtn").on("click", function() {
    let taskList = [];
    function saveTask()
        let task = {
            activity = document.getElementbyID("#9amTask").value
        }
      taskList.push(task);
      console.log(task);
      localStorage.setItem("MyTaskList", tasklist);
      $(".container").text(tasklist);
    });



    <script src="moment.min.js"></script>

      $(document).ready(function() {
        var dateAndTime = moment();
        var dateAndTime2 = dateAndTime.format('MMMM Do YYYY, h:mm:ss a');
          $("#currentDay").text(dateAndTime2);
          });