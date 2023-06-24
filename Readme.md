This is a complementary final project for the Numerical Analysis subject of the 2nd year of the Computer Science degree in the Faculty of Mathematics and Computing (MatCom) of Havana University, Cuba.

Given a set of n points (x<sub>i</sub>,y<sub>i</sub>) with i between 1 and n, and y<sub>i</sub> = f(x<sub>i</sub>) + e<sub>i</sub>, for a value of e<sub>i</sub> in [-1,1], the goal is to implement a visual application which allows to show the data and build a smoothing spline that "better adjusts to this data". The smoothing splines have a parameter. The application must allow the user to modify that parameter and automatically see the change in the splines.

For this purpose I used Python as the programming language of choice, due to its powerful libraries for data analysis. Of these, matplotlib was used for data visualization, together with ipywidgets for user interactivity, numpy as a fundamental package for scientific computing in Python, and scipy. This last one provided me with powerful implemented tools for interpolation with smoothing splines, such as:

- splrep: Find the B-spline representation of a 1-D curve. Given the set of data points (x[i], y[i]) determine a smooth spline approximation of degree k on the interval xb <= x <= xe.

- UnivariateSpline: 1-D smoothing spline fit to a given set of data points. Fits a spline y = spl(x) of degree k to the provided x, y data. s specifies the number of knots by specifying a smoothing condition.

