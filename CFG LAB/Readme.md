# Jonah Ball 40178421

## 1.


![Picture2](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-darealstyl/assets/78319780/3a508f99-aa5a-43ae-9c61-bacba9ce2900)


## 2.
Test Path 1: Trigger onClick with view.getId() returning R.id.key_0_btn.

Test Path 2: Trigger onClick with view.getId() returning R.id.key_1_btn.

Test Path 3: Trigger onClick with view.getId() returning R.id.key_2_btn.

Test Path 4: Trigger onClick with view.getId() returning R.id.key_3_btn.

Test Path 5: Trigger onClick with view.getId() returning R.id.key_4_btn.

Test Path 6: Trigger onClick with view.getId() returning R.id.key_5_btn.

Test Path 7: Trigger onClick with view.getId() returning R.id.key_6_btn.

Test Path 8: Trigger onClick with view.getId() returning R.id.key_7_btn.

Test Path 9: Trigger onClick with view.getId() returning R.id.key_8_btn.

Test Path 10: Trigger onClick with view.getId() returning R.id.key_9_btn.

Test Path 11: Trigger onClick with view.getId() returning R.id.key_add_btn.

Test Path 12: Trigger onClick with view.getId() returning R.id.key_sub_btn.

Test Path 13: Trigger onClick with view.getId() returning R.id.key_div_btn.

Test Path 14: Trigger onClick with view.getId() returning R.id.key_mult_btn.

Test Path 15: Trigger onClick with view.getId() returning R.id.key_clear_btn.

Test Path 16: Trigger onClick with view.getId() returning R.id.key_equals_btn, with symbol being "+".

Test Path 17: Trigger onClick with view.getId() returning R.id.key_equals_btn, with symbol being "-".

Test Path 18: Trigger onClick with view.getId() returning R.id.key_equals_btn, with symbol being "/".

Test Path 19: Trigger onClick with view.getId() returning R.id.key_equals_btn, with symbol being "*".

## 3.
Test Path 1: Start → onClick → R.id.key_0_btn → END

Test Path 2: Start → onClick → R.id.key_1_btn → END

Test Path 3: Start → onClick → R.id.key_2_btn → END

Test Path 4: Start → onClick → R.id.key_3_btn → END

Test Path 5: Start → onClick → R.id.key_4_btn → END

Test Path 6: Start → onClick → R.id.key_5_btn → END

Test Path 7: Start → onClick → R.id.key_6_btn → END

Test Path 8: Start → onClick → R.id.key_7_btn → END

Test Path 9: Start → onClick → R.id.key_8_btn → END

Test Path 10: Start → onClick → R.id.key_9_btn → END

Test Path 11: Start → onClick → R.id.key_add_btn → END

Test Path 12: Start → onClick → R.id.key_sub_btn → END

Test Path 13: Start → onClick → R.id.key_div_btn → END

Test Path 14: Start → onClick → R.id.key_mult_btn → END

Test Path 15: Start → onClick → R.id.key_clear_btn → END

Test Path 16: Start → onClick → R.id.key_equals_btn → symbol.equals("+") → END

Test Path 17: Start → onClick → R.id.key_equals_btn → symbol.equals("-") → END

Test Path 18: Start → onClick → R.id.key_equals_btn → symbol.equals("/") → END

Test Path 19: Start → onClick → R.id.key_equals_btn → symbol.equals("*") → END


## 4.
Test Requirements (TR) for Edge-Pair Coverage:

•	For the digit buttons (0-9):

  •	Each edge from the onClick to R.id.key_[0-9]_btn, and then directly to the END.

•	_*For the operation buttons (+, -, /, ):

  •	Each edge from the onClick to R.id.key_[operation]_btn, followed by a digit button, and then directly to the END.

•	For the clear button (CLR):

  •	The edge from the onClick to R.id.key_clear_btn and then directly to the END.

•	For the equals button (=):

  •	The edge from the onClick to R.id.key_equals_btn and then to the second switch(symbol) statement.

  •	Each pair of edges from the symbol decision to each operation within the second switch.

Test Paths (TP) for Edge-Pair Coverage:

•	For the digit buttons (0-9):

  •	TP1: Start → onClick → R.id.key_0_btn → END

  •	(Repeat TP1 for buttons 1 through 9.)

•	*For the operation buttons (+, -, /, ), after entering a digit:

  •	TP11: Start → onClick → R.id.key_0_btn → onClick → R.id.key_add_btn → END

  •	(Repeat TP11 for operations SUB, DIV, MUL after pressing a digit.)

•	For the clear button (CLR):

  •	TP15: Start → onClick → R.id.key_clear_btn → END

•	For the equals button (=), after entering a number and selecting an operation:

  •	TP16: Start → onClick → R.id.key_0_btn → onClick → R.id.key_add_btn → onClick → R.id.key_equals_btn → symbol.equals("+") → END

  •	TP17: Start → onClick → R.id.key_0_btn → onClick → R.id.key_sub_btn → onClick → R.id.key_equals_btn → symbol.equals("-") → END

  •	TP18: Start → onClick → R.id.key_0_btn → onClick → R.id.key_div_btn → onClick → R.id.key_equals_btn → symbol.equals("/") → END

  •	TP19: Start → onClick → R.id.key_0_btn → onClick → R.id.key_mult_btn → onClick → R.id.key_equals_btn → symbol.equals("*") → END


## 5.
![Picture1](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-darealstyl/assets/78319780/67a2e74b-a6a2-4dbf-a6aa-332a9397ae63)
