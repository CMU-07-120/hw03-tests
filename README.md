# Tests (for everyone!)

## In-class Exercise (paired)

1. Clone this Repo.

2. Pick at least 1 test folder in this repo to test your buggy code against (*HW3*).

   * You'll get familiar with running C0 code using paths, for example:

     ```
     cc0 -o sort-test <Path to lib>/*.c0 <Path to program> <Path to another student tests>
     ```

     Here's one that I ran:

     ```sh
     cc0 -o sort3-test homework-3-<name>/lib/*.c0 homework-3-<name>/sort1.c0 hw03-tests/1/sort1-test.c0
     ```

   * However, not everything is easy :). People's tests are all over the place.
     Some print answers, others have asserts. Some people tested on specific
     favorites, that you're file wouldn't have. So, you **will have to modify**
     things and fix up paths to align. You'll also have to make sure
     `favorites.txt` has the right path from where you run things, if a test
     suite relied on it.

     **Definitely review these tests and plan out** how you want to make this
     work.

3. After you've formed a test suite by choosing and modifying your classmates'
   tests and then running your buggy sorts (1-3) on them, append all of results
   to a single file. For example, if I've compiled my buggy sort1.c0 with
   someone's test on sort1, i.e. sort1-test.c0, I can run:

   ```sh
   ./sort1-test  &> results.txt
   ```

4. Once you have your results file with all the passes/failures,
   you can `cat` the file and pipe it into `grep` to list out
   all your failures and use `wc -l` to give us the count.
   Obviously, double-check this file that it's actually
   informative :).

5. It's hard to remember all the commands you've needed
   for steps 1-4 to work! And, shell histories only last for so long.
   Please log all of the commands you used that would make
   this process repeatable so that you can use it in the future.

6. Repeat 1-4 for 5 more test folders, to use as an extended
   test suite for your buggy code.

7. At the end of class, send us your log of commands and your results file.

## Commands that will be helpful:

* `cp`
* `mv`
* `ls`
* `cat`
* `grep`
* `wc`

