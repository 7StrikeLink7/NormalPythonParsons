---
layout: default
title: Subprograms (Functions and Procedures)
---


Random Item Procedure:
![image](https://user-images.githubusercontent.com/68385109/232054704-22003b28-fd77-4b89-b1f8-aee4f674a0ee.png)
<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "import random\n" +
    "superRareItem = 3\n" +
    "rareItem = 43\n" +
    "def pullItem():\n" +
    "  randomNumber = $$toggle::random$$.randint(0,100)\n" +
    "  print(randomNumber)\n" +
    "  #if random number is equal or lower than the number for super rare item\n" +
    "  if (randomNumber &lt;= superRareItem):\n" +
    "    print(&quot;You pulled a Super Rare Item! :D&quot;)\n" +
    "  # otherwise check random number between the values of super rare and rare item\n" +
    "  elif (randomNumber &gt; superRareItem) and (randomNumber &lt;= rareItem):\n" +
    "    print(&quot;you pulled a rare item!&quot;)\n" +
    "    \n" +
    "  #Else, any other number is a common item\n" +
    "  else:\n" +
    "    print(&quot;you pulled a common item.&quot;)\n" +
    " \n" +
    "#Main Body: calling the procedure\n" +
    "pullItem()";
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


![image](https://user-images.githubusercontent.com/68385109/216831738-bc7175e5-1360-4d00-b2f7-03ed00284e29.png)
![image](https://user-images.githubusercontent.com/68385109/216831731-692b7310-cc28-477b-ad1f-643e26dccabf.png)
<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def five():\n" +
    "  print(&quot;ooooooooooo&quot;)\n" +
    "  print(&quot;o         o&quot;)\n" +
    "  print(&quot;o  #   #  o&quot;)\n" +
    "  print(&quot;o    #    o&quot;)\n" +
    "  print(&quot;o  #   #  o&quot;)\n" +
    "  print(&quot;o         o&quot;)\n" +
    "  print(&quot;ooooooooooo&quot;)\n" +
    "#Main Program\n" +
    "five()";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "1-sortableTrash"
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

Function:
![image](https://user-images.githubusercontent.com/68385109/232056410-ef1f6845-3657-41c0-ad58-e81b52132dbf.png)

<div id="2-sortableTrash" class="sortable-code"></div> 
<div id="2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "#Creating a function to reverse your input\n" +
    "def reverseSentence(name):\n" +
    "  reversed = name[::-1]\n" +
    "  return reversed\n" +
    "#Main body\n" +
    "myName = input(&quot;What is your name? &quot;)\n" +
    "print(&quot;Your name backwards is:&quot;, reverseSentence(myName))\n" +
    "  ";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "2-sortable",
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
  $("#2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#2-feedbackLink").click(function(event){ 
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
