---
layout: default
title: While Loops - Cracking the safe
---

![image](https://user-images.githubusercontent.com/68385109/232052965-66468b10-030b-40a0-a80e-9de1964ec71f.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;Agent, the safe is behind the painting.&quot;)\n" +
    "attempts = 3\n" +
    "secretPassword = &quot;Skyfall&quot;\n" +
    "myGuess = &quot;&quot;\n" +
    "while (attempts &gt; 0) and (myGuess != secretPassword):\n" +
    "  print(&quot;Safe: Enter the password&quot;)\n" +
    "  myGuess = input()\n" +
    "  if ($$toggle::myGuess$$ == secretPassword):\n" +
    "    print(&quot;The safe has been opened. Good job agent.&quot;)\n" +
    "    \n" +
    "  else:\n" +
    "    print(&quot;Incorrect.&quot;)\n" +
    "    attempts = $$toggle::attempts$$ - 1\n" +
    "    print(&quot;Attempts Remaining: &quot;, attempts)\n" +
    "print(&quot;Time to go.&quot;)\n" +
    "  \n" +
    "  ";
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
