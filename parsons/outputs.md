# Easy Parsons: Outputs

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

[Outputs]
[Variables and Outputs]
[Variables, Outputs, and Inputs ]
[Maths Operators (input integers)]
[Random numbers]
[Strings and Casting]
[Booleans]
[If]
[If/Else]
[If/Elif/Else]
[Nested Ifs]
[For loops]
[While loops]
[Nested loops]
[Arrays/Lists]
[2D Lists]
[File handling]
[Subprograms(functions/procedures)]
