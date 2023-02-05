---
layout: default
title: Nested If statements
---

![image](https://user-images.githubusercontent.com/68385109/216828663-aa07420d-f966-4c61-91c6-94b80650ab79.png)

<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "likeMovies = input(&quot;Do you like movies? y/n &quot;)\n" +
    "if (likeMovies == &quot;y&quot;):\n" +
    "  favMovie = input(&quot;Cool! What is your favourite movie? &quot;)\n" +
    "  if (favMovie == &quot;Titanic&quot;):\n" +
    "    print(&quot;That is my favourite too!&quot;)\n" +
    "  else:\n" +
    "    print(&quot;Not a bad movie!&quot;)\n" +
    "else: \n" +
    "  print(&quot;That is a shame.&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#feedbackLink").click(function(event){ 
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
