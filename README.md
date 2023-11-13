# Tests (for everyone!)

## In-class Exercise

1. Clone this Repo.

2. Pick at least 6 test folders in this repo to use as your larger
   test suite on your buggy code from *HW3*.

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

3. After you've formed a test suite by choosing and modifying your classmates'
   tests and then running your buggy sorts (1-3) on them, append all of results
   to a single file. For example, if I've compiled my buggy sort1.c0 with
   someone's test on sort1, i.e. sort1-test.c0, I can run:

   ```sh
   ./sort1-test  >> results.txt
   ```

   The `>>` appends to a file (vs `>`).

4. Once you have your results file with all the passes/failures,
   you can `cat` the file and pipe it into `grep` to list out
   all your failures and use `wc -l` to give us the count.
   Obviously, double-check this file that it's actually
   informative :).


## Commands that will be helpful:

* `cp`
* `mv`
* `ls`
* `cat`
* `grep`
* `wc`

