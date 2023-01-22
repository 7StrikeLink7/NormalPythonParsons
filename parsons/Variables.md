# Variables and Outputs

 
![image](https://user-images.githubusercontent.com/68385109/213943796-df7dfd55-fb2f-4d77-95ef-c7ba82a626e3.png)

<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "myName = &quot;John&quot;\n" +
    "print(&quot;The variable myName takes the value of whaterver is to the right of the =.&quot;)\n" +
    "print(&quot;Hello,&quot;, myName, &quot;!&quot;)\n" +
    "print(&quot;Nice to meet you.&quot;)";
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
