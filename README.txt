The code was full of those variables which are of no use, they were declared in the function but never used in that function.
Similiarly some functions were getting the whole data from request but was using just one enitity, like $input = $request->all , and just using $input->name, so it can directly called $request->name, to avoid loading the data which is of no use.
Some of the functions were using if else conditions, I minimize them to ternary operators.
Similarly some functions were repeadly using the same functionality, i created the private function for it, to minimize the code and to use that functionality multiple times.
Comments were added, i removed them.
Some code was commented, I removed it.
These were the points which i noticed and cleared maximum of them, obv the repository file is of 1600 lines, but initially, i have refactored maximum code.