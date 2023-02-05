---
layout: default
title: Selection – IF Elif Else statements - Menu Select
---

![image](https://user-images.githubusercontent.com/68385109/214693957-e05079c1-1365-4968-ae00-cddd0052c67d.png)

 <div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#Display menu\n" +
    "print(&quot;Menu:&quot;)\n" +
    "print(&quot;a. Start&quot;)\n" +
    "print(&quot;b. Load&quot;)\n" +
    "print(&quot;c. Settings&quot;)\n" +
    "userChoice = input(&quot;Enter a corresponding letter for what you want to do: &quot;)\n" +
    "userChoice = userChoice.lower() #making input into lowercase\n" +
    "#Display scenario from user&#039;s choice\n" +
    "if (userChoice == &quot;a&quot;):\n" +
    "  print(&quot;Starting Game&quot;)\n" +
    "elif(userChoice == &quot;b&quot;):\n" +
    "  print(&quot;Loading save file&quot;)\n" +
    "elif(userChoice == &quot;c&quot;):\n" +
    "  print(&quot;This is the settings&quot;)\n" +
    "else:\n" +
    "  print(&quot;Sorry try again.&quot;)\n" +
    "  ";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "0-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#0-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#0-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
## Topics:
[Outputs](./Outputs.html)
[Variables and Outputs](./Variables.html)
[Variables, Outputs, and Inputs](./Inputs.html)
[Maths Operators (input integers)](./Maths.html)
[Random numbers](./Random.html)
[Strings and Casting](./Casting.html)
[Booleans](./Booleans.html)
[If](./If.html)
[If/Else](./Else.html)
[If/Elif/Else](./Elif.html)
[Nested Ifs](./NestedIf.html)
[For loops](./For.html)
[While loops](./While.html)
[Nested loops](./NestedLoops.html)
[Arrays/Lists](./Arrays.html)
[2D Lists](./2D.html)
[File handling](./Files.html)
[Subprograms(functions/procedures)](./Subprograms.html)
