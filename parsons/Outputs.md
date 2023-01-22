# Easy Parsons: Outputs
![image](https://user-images.githubusercontent.com/68385109/213943936-ea88d7cd-6b0d-4013-89e5-85c071c5a4ff.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(&quot;First, read all the lines.&quot;)\n" +
    "print(&quot;Second, Cut and Copy lines into the right order.&quot;)\n" +
    "print(&quot;Third, take a screenshot.&quot;)\n" +
    "print(&quot;Lastly, give yourself a pat on the back.&quot;)";
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
[Outputs](./parsons/Outputs.html)
[Variables and Outputs](./parsons/Variables.html)
[Variables, Outputs, and Inputs](./parsons/Inputs.html)
[Maths Operators (input integers)](./parsons/Inputs.html)
[Random numbers](./parsons/Random.html)
[Strings and Casting](./parsons/Casting.html)
[Booleans](./parsons/Booleans.html)
[If](./parsons/If.html)
[If/Else](./parsons/Else.html)
[If/Elif/Else](./parsons/Elif.html)
[Nested Ifs](./parsons/NestedIf.html)
[For loops](./parsons/For.html)
[While loops](./parsons/While.html)
[Nested loops](./parsons/NestedLoops.html)
[Arrays/Lists](./parsons/Arrays.html)
[2D Lists](./parsons/2D.html)
[File handling](./parsons/Files.html)
[Subprograms(functions/procedures)](./parsons/Subprograms.html)
