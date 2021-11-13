# Ruhi-P-B
<center><h3>Tic Tac Toe:</h3>
<SCRIPT>



//if IE4/NS6, apply style
if (document.all||document.getElementById){
document.write('<style>.tictac{')
document.write('width:50px;height:50px;')
document.write('}</style>')
}

var sqr1
var sqr2
var sqr3
var sqr4
var sqr5
var sqr6
var sqr7
var sqr8
var sqr9
var sqr1T = 0
var sqr2T = 0
var sqr3T = 0
var sqr4T = 0
var sqr5T = 0
var sqr6T = 0
var sqr7T = 0
var sqr8T = 0
var sqr9T = 0
var moveCount = 0
var turn = 0
var mode = 1

function vari()
{
sqr1 = document.tic.sqr1.value
sqr2 = document.tic.sqr2.value
sqr3 = document.tic.sqr3.value
sqr4 = document.tic.sqr4.value
sqr5 = document.tic.sqr5.value
sqr6 = document.tic.sqr6.value
sqr7 = document.tic.sqr7.value
sqr8 = document.tic.sqr8.value
sqr9 = document.tic.sqr9.value
}
function check()
{
  if(sqr1 == " X " && sqr2 == " X " && sqr3 == " X ")
  {
    alert("You Win!")
    reset()
  } 
  else if(sqr4 == " X " && sqr5 == " X " && sqr6 == " X ")
  {
    alert("You Win!")
    reset()
  } 
  else if(sqr7 == " X " && sqr8 == " X " && sqr9 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr1 == " X " && sqr4 == " X " && sqr7 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr2 == " X " && sqr5 == " X " && sqr8 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr3 == " X " && sqr6 == " X " && sqr9 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else if(sqr3 == " X " && sqr5 == " X " && sqr7 == " X ")
  {
    alert("You Win!")
    reset()
  }
  else
  {
    winCheck()
    check2()
    drawCheck()  
  } 
}

function check2()
{
  vari()
  drawCheck()
  if(sqr1 == " O " && sqr2 == " O " && sqr3 == " O ")
  {
    alert("You Lose!")
    reset()
  } 
  else if(sqr4 == " O " && sqr5 == " O " && sqr6 == " O ")
  {
    alert("You Lose!")
    reset()
  } 
  else if(sqr7 == " O " && sqr8 == " O " && sqr9 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr1 == " O " && sqr4 == " O " && sqr7 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr2 == " O " && sqr5 == " O " && sqr8 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr3 == " O " && sqr6 == " O " && sqr9 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9 == " O ")
  {
    alert("You Lose!")
    reset()
  }
  else if(sqr3 == " O " && sqr5 == " O " && sqr7 == " O ")
  {
    alert("You Lose!")
    reset()
  }
}

function player1Check()
{
  if(sqr1 == " X " && sqr2 == " X " && sqr3 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  } 
  else if(sqr4 == " X " && sqr5 == " X " && sqr6 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  } 
  else if(sqr7 == " X " && sqr8 == " X " && sqr9 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr1 == " X " && sqr4 == " X " && sqr7 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr2 == " X " && sqr5 == " X " && sqr8 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr3 == " X " && sqr6 == " X " && sqr9 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else if(sqr3 == " X " && sqr5 == " X " && sqr7 == " X ")
  {
    alert("Player 1 wins!")
    reset()
  }
  else
  {
    player2Check()
    drawCheck()  
  } 
}

function player2Check()
{
  vari()
  drawCheck()
  if(sqr1 == " O " && sqr2 == " O " && sqr3 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  } 
  else if(sqr4 == " O " && sqr5 == " O " && sqr6 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  } 
  else if(sqr7 == " O " && sqr8 == " O " && sqr9 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr1 == " O " && sqr4 == " O " && sqr7 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr2 == " O " && sqr5 == " O " && sqr8 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr3 == " O " && sqr6 == " O " && sqr9 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
  else if(sqr3 == " O " && sqr5 == " O " && sqr7 == " O ")
  {
    alert("Player 2 wins!")
    reset()
  }
}

function drawCheck()
{
  vari()
  moveCount = sqr1T + sqr2T + sqr3T + sqr4T + sqr5T + sqr6T + sqr7T + sqr8T + sqr9T 
  if(moveCount == 9)
  {
    reset()
    alert("Draw") 
  }
}

function winCheck()
{
  check2()
  if(sqr1 == " O " && sqr2 == " O " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr2 == " O " && sqr3 == " O " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr4 == " O " && sqr5 == " O " && sqr6T == 0 && turn == 1)
  {
    document.tic.sqr6.value = " O "
    sqr6T = 1;
    turn = 0;
  }
  else if(sqr5 == " O " && sqr6 == " O " && sqr4T == 0 && turn == 1)
  {
    document.tic.sqr4.value = " O "
    sqr4T = 1;
    turn = 0;
  }
  else if(sqr7 == " O " && sqr8 == " O " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr8 == " O " && sqr9 == " O " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr5 == " O " && sqr9 == " O " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr3 == " O " && sqr5 == " O " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr7 == " O " && sqr5 == " O " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr3 == " O " && sqr2T == 0 && turn == 1)
  {
    document.tic.sqr2.value = " O "
    sqr2T = 1;
    turn = 0;
  }
  else if(sqr4 == " O " && sqr6 == " O " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr7 == " O " && sqr9 == " O " && sqr8T == 0 && turn == 1)
  {
    document.tic.sqr8.value = " O "
    sqr8T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr7 == " O " && sqr4T == 0 && turn == 1)
  {
    document.tic.sqr4.value = " O "
    sqr4T = 1;
    turn = 0;
  }
  else if(sqr2 == " O " && sqr8 == " O " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr3 == " O " && sqr9 == " O " && sqr6T == 0 && turn == 1)
  {
    document.tic.sqr6.value = " O "
    sqr6T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr5 == " O " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr4 == " O " && sqr7 == " O " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr5 == " O " && sqr8 == " O " && sqr2T == 0 && turn == 1)
  {
    document.tic.sqr2.value = " O "
    sqr2T = 1;
    turn = 0;
  }
  else if(sqr6 == " O " && sqr9 == " O " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr4 == " O " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr2 == " O " && sqr5 == " O " && sqr8T == 0 && turn == 1)
  {
    document.tic.sqr8.value = " O "
    sqr8T = 1;
    turn = 0;
  }
  else if(sqr3 == " O " && sqr6 == " O " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr1 == " O " && sqr9 == " O " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr3 == " O " && sqr7 == " O " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else
  {
    computer()
  }
  check2()
}
function computer()
{
  check2()
  if(sqr1 == " X " && sqr2 == " X " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr2 == " X " && sqr3 == " X " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr4 == " X " && sqr5 == " X " && sqr6T == 0 && turn == 1)
  {
    document.tic.sqr6.value = " O "
    sqr6T = 1;
    turn = 0;
  }
  else if(sqr5 == " X " && sqr6 == " X " && sqr4T == 0 && turn == 1)
  {
    document.tic.sqr4.value = " O "
    sqr4T = 1;
    turn = 0;
  }
  else if(sqr7 == " X " && sqr8 == " X " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr8 == " X " && sqr9 == " X " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr5 == " X " && sqr9 == " X " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr3 == " X " && sqr5 == " X " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr7 == " X " && sqr5 == " X " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr3 == " X " && sqr2T == 0 && turn == 1)
  {
    document.tic.sqr2.value = " O "
    sqr2T = 1;
    turn = 0;
  }
  else if(sqr4 == " X " && sqr6 == " X " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr7 == " X " && sqr9 == " X " && sqr8T == 0 && turn == 1)
  {
    document.tic.sqr8.value = " O "
    sqr8T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr7 == " X " && sqr4T == 0 && turn == 1)
  {
    document.tic.sqr4.value = " O "
    sqr4T = 1;
    turn = 0;
  }
  else if(sqr2 == " X " && sqr8 == " X " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr3 == " X " && sqr9 == " X " && sqr6T == 0 && turn == 1)
  {
    document.tic.sqr6.value = " O "
    sqr6T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr5 == " X " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr4 == " X " && sqr7 == " X " && sqr1T == 0 && turn == 1)
  {
    document.tic.sqr1.value = " O "
    sqr1T = 1;
    turn = 0;
  }
  else if(sqr5 == " X " && sqr8 == " X " && sqr2T == 0 && turn == 1)
  {
    document.tic.sqr2.value = " O "
    sqr2T = 1;
    turn = 0;
  }
  else if(sqr6 == " X " && sqr9 == " X " && sqr3T == 0 && turn == 1)
  {
    document.tic.sqr3.value = " O "
    sqr3T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr4 == " X " && sqr7T == 0 && turn == 1)
  {
    document.tic.sqr7.value = " O "
    sqr7T = 1;
    turn = 0;
  }
  else if(sqr2 == " X " && sqr5 == " X " && sqr8T == 0 && turn == 1)
  {
    document.tic.sqr8.value = " O "
    sqr8T = 1;
    turn = 0;
  }
  else if(sqr3 == " X " && sqr6 == " X " && sqr9T == 0 && turn == 1)
  {
    document.tic.sqr9.value = " O "
    sqr9T = 1;
    turn = 0;
  }
  else if(sqr1 == " X " && sqr9 == " X " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else if(sqr3 == " X " && sqr7 == " X " && sqr5T == 0 && turn == 1)
  {
    document.tic.sqr5.value = " O "
    sqr5T = 1;
    turn = 0;
  }
  else
  {
    AI()
  }
  check2()
}

function AI()
{
  vari()
  if(document.tic.sqr5.value == "     " && turn == 1)
  {
    document.tic.sqr5.value = " O "
    turn = 0
    sqr5T = 1
  }
  else if(document.tic.sqr1.value == "     " && turn == 1)
  {
    document.tic.sqr1.value = " O "
    turn = 0
    sqr1T = 1
  }
  else if(document.tic.sqr9.value == "     " && turn == 1)
  {
    document.tic.sqr9.value = " O "
    turn = 0
    sqr9T = 1
  }
  else if(document.tic.sqr6.value == "     " && turn == 1)
  {
    document.tic.sqr6.value = " O "
    turn = 0
    sqr6T = 1
  }
  else if(document.tic.sqr2.value == "     " && turn == 1)
  {
    document.tic.sqr2.value = " O "
    turn = 0
    sqr2T = 1
  }
  else if(document.tic.sqr8.value == "     " && turn == 1)
  {
    document.tic.sqr8.value = " O "
    turn = 0
    sqr8T = 1
  }
  else if(document.tic.sqr3.value == "     " && turn == 1)
  {
    document.tic.sqr3.value = " O "
    turn = 0
    sqr3T = 1
  }
  else if(document.tic.sqr7.value == "     " && turn == 1)
  {
    document.tic.sqr7.value = " O "
    turn = 0
    sqr7T = 1
  }
  else if(document.tic.sqr4.value == "     " && turn == 1)
  {
    document.tic.sqr4.value = " O "
    turn = 0
    sqr4T = 1
  }
  check2()
}

function reset()
{
  document.tic.sqr1.value = "     "
  document.tic.sqr2.value = "     "
  document.tic.sqr3.value = "     "
  document.tic.sqr4.value = "     "
  document.tic.sqr5.value = "     "
  document.tic.sqr6.value = "     "
  document.tic.sqr7.value = "     "
  document.tic.sqr8.value = "     "
  document.tic.sqr9.value = "     "
  sqr1T = 0
  sqr2T = 0
  sqr3T = 0
  sqr4T = 0
  sqr5T = 0
  sqr6T = 0
  sqr7T = 0
  sqr8T = 0
  sqr9T = 0
  vari()
  turn = 0
  moveCount = 0
}

function resetter()
{
  reset()
}
</SCRIPT>
<table>
<td>
<tr>
<FORM NAME="tic" method="post">
<INPUT TYPE="button" NAME="sqr1" class="tictac" value="     " onClick="if(document.tic.sqr1.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr1.value = ' X '; sqr1T = 1; turn = 1; vari(); check();} else if(document.tic.sqr1.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr1.value = ' X '; sqr1T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr1.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr1.value = ' O '; sqr1T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr2" class="tictac" value="     " onClick="if(document.tic.sqr2.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr2.value = ' X '; sqr2T = 1; turn = 1; vari(); check();} else if(document.tic.sqr2.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr2.value = ' X '; sqr2T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr2.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr2.value = ' O '; sqr2T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr3" class="tictac" value="     " onClick="if(document.tic.sqr3.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr3.value = ' X '; sqr3T = 1; turn = 1; vari(); check();} else if(document.tic.sqr3.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr3.value = ' X '; sqr3T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr3.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr3.value = ' O '; sqr3T = 1; turn = 1; vari(); player1Check()} drawCheck()"><br />
<INPUT TYPE="button" NAME="sqr4" class="tictac" value="     " onClick="if(document.tic.sqr4.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr4.value = ' X '; sqr4T = 1; turn = 1; vari(); check();} else if(document.tic.sqr4.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr4.value = ' X '; sqr4T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr4.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr4.value = ' O '; sqr4T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr5" class="tictac" value="     " onClick="if(document.tic.sqr5.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr5.value = ' X '; sqr5T = 1; turn = 1; vari(); check();} else if(document.tic.sqr5.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr5.value = ' X '; sqr5T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr5.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr5.value = ' O '; sqr5T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr6" class="tictac" value="     " onClick="if(document.tic.sqr6.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr6.value = ' X '; sqr6T = 1; turn = 1; vari(); check();} else if(document.tic.sqr6.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr6.value = ' X '; sqr6T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr6.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr6.value = ' O '; sqr6T = 1; turn = 1; vari(); player1Check()} drawCheck()"><br />
<INPUT TYPE="button" NAME="sqr7" class="tictac" value="     " onClick="if(document.tic.sqr7.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr7.value = ' X '; sqr7T = 1; turn = 1; vari(); check();} else if(document.tic.sqr7.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr7.value = ' X '; sqr7T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr7.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr7.value = ' O '; sqr7T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr8" class="tictac" value="     " onClick="if(document.tic.sqr8.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr8.value = ' X '; sqr8T = 1; turn = 1; vari(); check();} else if(document.tic.sqr8.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr8.value = ' X '; sqr8T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr8.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr8.value = ' O '; sqr8T = 1; turn = 1; vari(); player1Check()} drawCheck()">
<INPUT TYPE="button" NAME="sqr9" class="tictac" value="     " onClick="if(document.tic.sqr9.value == '     ' && turn == 0 && mode == 1) {document.tic.sqr9.value = ' X '; sqr9T = 1; turn = 1; vari(); check();} else if(document.tic.sqr9.value == '     ' && turn == 1 && mode == 2) {document.tic.sqr9.value = ' X '; sqr9T = 1; turn = 0; vari(); player1Check()} else if(document.tic.sqr9.value == '     ' && turn == 0 && mode == 2) {document.tic.sqr9.value = ' O '; sqr9T = 1; turn = 1; vari(); player1Check()} drawCheck()">
</table>
</form>
<hr>
<h3>Guess The Number:</h3>
<SCRIPT LANGUAGE="JavaScript">
<!-- ;
// numberguess is by Lancer - written 4 Jan 1999
// lancer@kp.planet.gen.nz

var guessme=Math.round(Math.random()*(99)+1);
var speech='Guess my number (from 1 to 100)';

function process(mystery) {
var guess=document.forms.guessquiz.guess.value;
var speech='"'+guess+ '" does not make sense to me.';
document.forms.guessquiz.guess.value='';

if (guess==mystery)
{
document.forms.guessquiz.prompt.value='Congratulations! '+mystery+' is correct!';
alert ('The mystery number is '+mystery+'! \n\nPress this button to reload the page for another game.');
speech='';
document.location=document.location;
}

if (mystery<guess)
{
speech='Less than '+ guess;
}

if (mystery>guess)
{
speech='Greater than '+ guess;
}

if (guess=='')
{
speech='You didn\'t guess anything!'
}

document.forms.guessquiz.prompt.value=speech; document.forms.guessquiz.guess.focus();

}

// end hide -->
</SCRIPT>

<FORM onSubmit="" NAME="guessquiz">
<CENTER>
<TABLE ALIGN="CENTER" BGCOLOR="#888888" BORDER="3" CELLPADDING="5">
<TR>
<TD BGCOLOR="#004080">
<FONT COLOR="#ffffff" FACE="Arial"><B>GUESS THE NUMBER (1 - 100)</B></FONT>
</TD>
</TR>
<TR>
<TD>
<CENTER>
<INPUT TYPE="text" NAME="prompt" SIZE="41" MAXLENGTH="40" VALUE="Guess the number (from 1 to 100)"><BR>
<INPUT TYPE="text" pattern="[0-9]*" NAME="guess" SIZE="4" MAXLENGTH="3" VALUE="">
<INPUT TYPE="button" VALUE="Guess" onClick='process(guessme)'>
</CENTER>
</TD>
</TR>
</TABLE>
</CENTER>
</FORM>
<hr>
<h3>Russian Roulette:<h3>
<table border="0" width="350" cellspacing="0" cellpadding="0">
  <tr>
    <td></td>
    <td>

<form name="fire">
Load number of bullets (1-6):<br /><input name="bullets" type="text" size=3 value=2><br />

<p>
<input name="message" type="button" value="Play Roulette!" onClick="fireit()">
</p>

</form>

<script>

//Russian Roulette Game- by javascriptkit.com
//Visit JavaScript Kit (http://javascriptkit.com) for script
//Credit must stay intact for use

function fireit(){
var theone=Math.floor(Math.random()*6)

if (theone<=document.fire.bullets.value-1)
alert("Bang. You\'re dead!")
else{
document.fire.message.value="Whew. Got lucky!"
setTimeout("document.fire.message.value='Play Roulette'",500)
}
}

</script>



</td>
  </tr>
</table>
</center><hr>
<h3>Race Track</h3>
<!DOCTYPE html>
<html>
<script>
var interval = {};
function initMovement(car, speed) 
{
    var carObj = document.getElementById(car);
    var left = 0;
    interval[car] = setInterval(function()
    {
        left += speed/100;
        carObj.style.left = left+"px";
        
        if(left >= 210) //finish
        {
            for(var i in interval) 
            {
                clearInterval(interval[i]);
            }
            document.getElementById("start").disabled = false;
            document.getElementById("stop").disabled = true;
        }
    },10);
}
function start() 
{
    var speed1 = document.getElementById("speed1").value;
    var speed2 = document.getElementById("speed2").value;
    initMovement("car1", speed1);
    initMovement("car2", speed2);
    document.getElementById("start").disabled = true;
    document.getElementById("stop").disabled = false;
}
function stop() 
{
    for(var i in interval) 
    {
        clearInterval(interval[i]);
    }
    document.getElementById("start").disabled = false;
    document.getElementById("stop").disabled = true;
}
</script>
<style>#container 
{
    width:280px;
}
#car1
{
    background-color:red;
    position:relative;
    width:60px;
    height:30px;
    border:none;
   
}
#car2
{
    background-color:green;
    position:relative;
    width:60px;
    height:30px;
    border:none;
    
} 
#road 
{
    padding:10px;
    background-color:#484848;
}
#separator 
{
    height:7px;
    background-color:white;
    margin-top:10px;
    margin-bottom:10px;
}
#controls
{
    padding:10px;
    text-align:center;
}

</style>
<head>

</head>
<body>
    <div id="container">
        <div id="road">
            <div id="car1"></div>
            <div id="separator"></div>
            <div id="car2"></div>
        </div>
        <div id="controls">
            <label>Car1 Speed (px/sec.): </label>
            <input type="text" pattern="[0-9]*"id="speed1" value="100"/>
            <br><br>
            <label>Car2 Speed (px/sec.): </label>
            <input type="text" pattern="[0-9]*" id="speed2" value="80"/>
            <br><br>
            <button id="start" onclick="start()">START</button>
            <button id="stop" onclick="stop()">STOP</button>
        </div>
    </div>
</body>
</html>
