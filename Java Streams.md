# Java Streams Examples

**Question 1:** Find the first non repeated letter from a string.
**Example:** If string is `abcabde` ->> Then answer will be `c`
<details>
  <summary>**Click here to show the solution**</summary>
  ```
Stream.of(str.split("")).filter(ch -> str.indexOf(ch, str.indexOf(ch) + 1) == -1).findFirst()
  ```
  </details>