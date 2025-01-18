# Assignment 1:
## Stretchy Words

Sometimes people repeat letters to represent extra feeling, such as "hello" -> "heeellooo", "hi" -> "hiiii". In these strings like "heeellooo", we have groups of adjacent letters that are all the same: "h", "eee", "ll", "ooo".

For some given string S, a query word is stretchy if it can be made to be equal to S by any number of applications of the following extension operation: choose a group consisting of characters c, and add some number of characters c to the group so that the size of the group is 3 or more.

For example, starting with "hello", we could do an extension on the group "o" to get "hellooo", but we cannot get "helloo" since the group "oo" has size less than 3. Also, we could do another extension like "ll" -> "lllll" to get "helllllooo". If S = "helllllooo", then the query word "hello" would be stretchy because of these two extension operations: query = "hello" -> "hellooo" -> "helllllooo" = S.

Given a list of query words, return the number of words that are stretchy.

### Example:
**Input:**
```
S = "heeellooo" words = ["hello", "hi", "helo"]
```
**Output:**
```
1
```
**Explanation:**  
We can extend "e" and "o" in the word "hello" to get "heeellooo".  
We can't extend "helo" to get "heeellooo" because the group "ll" is not size 3 or more.

### Constraints:

- `0 <= len(S) <= 100`
- `0 <= len(words) <= 100`
- `0 <= len(words[i]) <= 100`
- `S` and all words in `words` consist only of lowercase letters.

# Assignment 2:
## Prepare the Data

1. **Take a sufficient sample of Gutenberg's digital 3 books.**

2. **Create (random?!) samples of 200 partitions of the book.**  
   - Each partition or record should contain exactly **100 words**.

3. **Generalize the program**  
   - Ensure the program is capable of replicating this process for **multiple books**.

4. **Labeling**  
   - Maintain a label for each of the text segments, records, or documents.
   - Label them as **a, b, c, etc.** according to the book they belong to.

5. **Manipulations**  
   - Use **Regular Expressions** and **Pandas** for data manipulation.
   - Serialize the data for further use.
