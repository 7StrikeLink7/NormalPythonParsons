---
layout: default
title: Variables - Introduction
---
 

![image](https://user-images.githubusercontent.com/68385109/232027083-64cc72f5-0e0d-4f1a-8bd4-f68bc4aaf2ca.png)
<div id="1-sortableTrash" class="sortable-code"></div> 
<div id="1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "myName = &quot;John&quot;\n" +
    "numberOfSweets = 10\n" +
    "print(&quot;My name is&quot;, myName) \n" +
    "print(&quot;I bought some sweets.&quot;)\n" +
    "print(&quot;I have&quot;, numberOfSweets, &quot;sweets.&quot;)";
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
