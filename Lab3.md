#1 (a)
x = 2
function(x) {x} (8)
print x

Under ***static scoping, the following will print 2.
Under ***dynamic scoping, the following will print 8.

They yield different results because the environment changes when the function is called when evaluated using big steps rather than being substituted when evaluated with small steps.

#2 (c)
The evaluation order can be determined if the operation is small-step and if the code has side-effects. Otherwise, it is not possible to tell the evaluation order.

#3
The evaluation order is left to right for e1 + e2. To change the evaluation order, you would need to change the search rule in the small step to eval e1 instead of e2.

#4 (a)
if (x != null && x.isValid())

If there was no short-circuit rule for the above statement, then the second expression would be evaluated and the program would encounter a segmentation fault for attempting to dereference a NULL pointer.

#4 (b)
Yes, there is a short circuit because there is a search rule to handle the case when e1 evaluates to false.