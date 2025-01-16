# PHP Silent Array Key Access Bug

This repository demonstrates a common yet subtle bug in PHP: the silent failure when accessing a non-existent array key.  Accessing a key that doesn't exist returns `NULL` instead of throwing an error, which can be difficult to track down.

The `bug.php` file showcases the problem, and `bugSolution.php` provides a solution using `isset()` or `array_key_exists()` for robust key checking.

This issue often surfaces during data processing or when working with nested arrays, and the absence of an error makes it particularly sneaky!