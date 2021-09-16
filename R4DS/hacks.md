# R currated hacks

* fetch unique value for every column in data frame: `lapply(data, function(x) unique(x))`
* select() helper functions
  - starts_with('abc'): columns that start with pattern
  - ends_with('xyz'): columns that end with pattern
  - contains('pattern'): columns that contain pattern
  - matches('regex'): evaluating regex (pretty useful)
  - num_range('exam', 1:3): matching exam1,exam2 and exam3
