---
layout: default
title: Selection – IF Elif Else statements - Name Length
---

![image](https://user-images.githubusercontent.com/68385109/232047208-f73d077b-27d4-480b-a28d-4dcad97b33a2.png)
<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Hello mortal, I am pythongarobtrabatron v11112.&quot;)\n" +
    "name = input(&quot;What is your name? &quot;)\n" +
    "nameLength = len(name)\n" +
    "#Output different responses depending on name length\n" +
    "if nameLength &lt; 4: \n" +
    "  print(&quot;Wow, you have a short name!&quot;)\n" +
    "elif (nameLength &gt;= 4 and nameLength &lt; 7):\n" +
    "  print(&quot;I think that is an average length name!&quot;)\n" +
    "else:\n" +
    "  print(&quot;What a long name!&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
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


![image](https://user-images.githubusercontent.com/68385109/232049625-284f8228-2de6-4745-8e4b-4fd989337c04.png)

<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#Menu Selection at the overpriced cafe.\n" +
    "print(&quot;---MENU---\n1.Coffee\n2.Hot Chocolate\n3.Milk Tea\n4.Bubble Tea\n\n&quot;)\n" +
    "myChoice = int(input(&quot;What would you like to order? Enter number: &quot;))\n" +
    "if (myChoice == 1):\n" +
    "  print(&quot;A cup of coffee! Very nice. £100 please.&quot;)\n" +
    "elif (myChoice == 2):\n" +
    "  print(&quot;Hot Chocolate coming up! £30 please&quot;)\n" +
    "elif (myChoice == 3):\n" +
    "  print(&quot;Tea coming up! It is my specialty! So... £200 please!&quot;)\n" +
    "elif (myChoice == 4):\n" +
    "  print(&quot;Bubble Tea ... sorry, we ran out.&quot;)\n" +
    "else:\n" +
    "  print(&quot;Sorry, I didn&#039;t understand that. Good day.&quot;)\n" +
    "  ";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#1-feedbackLink").click(function(event){ 
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
