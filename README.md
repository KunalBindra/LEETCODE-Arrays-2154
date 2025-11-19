# LEETCODE-Arrays-2154
---

# ✔ **Input**

```
nums = [5, 3, 6, 1, 12]
original = 3
```

---

# ✔ **Step 1: Sort the array**

After
`Arrays.sort(nums);`

Array becomes:

```
[1, 3, 5, 6, 12]
```

---

# ✔ **Step 2: Loop through array**

We compare each element with `original`.

| i | nums[i] | original | nums[i] == original? | Action                     |
| - | ------- | -------- | -------------------- | -------------------------- |
| 0 | 1       | 3        | 1 == 3? ❌            | No change                  |
| 1 | 3       | 3        | 3 == 3? ✔            | original = 3 * 2 = **6**   |
| 2 | 5       | 6        | 5 == 6? ❌            | No change                  |
| 3 | 6       | 6        | 6 == 6? ✔            | original = 6 * 2 = **12**  |
| 4 | 12      | 12       | 12 == 12? ✔          | original = 12 * 2 = **24** |

---

# ✔ **Step 3: End of loop**

Final value of `original`:

```
24
```

---

# ⭐ **Final Output: 24**
