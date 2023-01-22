---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Multiple Parson's Problems on One Page
---
## Parsons Tutorial 
Problem:
Drag and re-arrange the blocks so to output: 

Hello!
This is a print statement.
The text in between the brackets get displayed to you.


<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(“Hello!&quot;)\n" +
    "print(“This is a print statement.&quot;)\n" +
    "print(“The text in between the brackets get displayed to you.”)";
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

### Example Next Link
[Next](./parsons/example1.html)

## Topics:
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

 
 

 
![image](https://user-images.githubusercontent.com/68385109/213919695-59481689-588f-4df1-8037-23c09f5bf6ac.png)

