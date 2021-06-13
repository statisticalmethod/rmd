Habits
================
John Doe
March 22, 2005

knit: (function(input\_file, encoding) { out\_dir &lt;- ‘docs’;
rmarkdown::render(input\_file, encoding=encoding,
output\_file=file.path(dirname(input\_file), out\_dir, ‘index.html’))})

## Simple Linear Regression

Here, the independent variable is assumed to have a single dimension,
and thus we are only looking towards estimating two coefficients. Let
*x*<sub>*i*</sub> be the *i*<sup>*t**h*</sup> observation and
*Y*<sub>*i*</sub> be the associated response, then

The mean squared error is used here as it is the natural error function
that emerges when we try to obtain MLE estimates of the coefficients. As
is visible from the fomulae for point estimates of coefficients, they
are linear combinations of normal variables (*Y*) and thus are normally
distributed.

Simple linear regression is discussed in detail in the probability notes
on this site. It also discusses confidence intervals for the
coefficients, the prediction intervals for the response and hypothesis
testing for relation between input and response.

### Coefficient of Determination

*R*<sup>2</sup> is often used as a metric for checking how good the
regression model is. It’s definition is invariant to the number of
independent variables A good model will explain most of the variance in
*Y* usig the input variables. Hence, *R*<sup>2</sup> close to 1 is a
good model and vice versa. ***R*<sup>2</sup> usually increases as more
and more variables are added to the model**.
