# find_zero
The first input argument is a “function handle”. All other arguments are scalar numbers, and x1 must be less than x2. The function finds an x that lies in the range from x1 to x2 such that after the command, y=f(x), is executed inside the function find_zero, y is approximately zero as defined by abs(y)<1e-10. The function f has one scalar input and one scalar output, and a plot of its values crosses the x-axis exactly once between x1 and x2 (see attached figure). It is the responsibility of the user to call the function with arguments that obey these rules.

Example run:
find_zero(@sin,-2.5,2.3) % as shown in the figure
ans =
     -6.4000e-11

Example run:
format long
find_zero(@cos,-2,1.3)
ans =
     -1.570796326871000
