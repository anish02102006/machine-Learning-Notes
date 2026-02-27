Sure! Let’s do a **detailed introduction to NumPy** in **Hinglish** so that concepts are clear and easy to remember. I’ll cover everything from basics, features, arrays, operations, and practical examples.

---

## **1. NumPy kya hai?**

**NumPy** ka full form hai **Numerical Python**.
Ye Python ka ek library hai jo **high-performance numerical computing** ke liye use hoti hai. Matlab agar aapko **mathematical operations, large data, arrays, matrices** efficiently handle karni hai, toh NumPy best hai.

**Key Points:**

* Ye **Python lists** se zyada fast hai.
* Ye **multi-dimensional arrays** support karta hai (1D, 2D, 3D…).
* Ye scientific computing ke liye **base library** hai (Matplotlib, Pandas, SciPy, ML libraries NumPy pe depend karte hain).

---

## **2. NumPy ke Features**

1. **Ndarray (N-dimensional array):**
   Efficient data storage aur fast operations ke liye **ndarray** ka use hota hai.

2. **Vectorized Operations:**
   Aap loops ke bina arrays pe **+ , -, *, /** operations kar sakte ho.

3. **Mathematical Functions:**
   Trigonometry, statistics, linear algebra sab built-in functions ke through possible hai.

4. **Memory Efficient:**
   Python lists ke comparison mein, NumPy arrays memory zyada efficiently use karte hain.

5. **Broadcasting:**
   Arrays of different shapes ke saath bhi operations possible hote hain.

---

## **3. NumPy install karna**

```bash
pip install numpy
```

Import karte hain:

```python
import numpy as np
```

**Tip:** Usually `np` alias use karte hain taaki code concise rahe.

---

## **4. NumPy Array (ndarray) kya hai?**

Python list ke jaisa hai, lekin **homogeneous data type** ka use karta hai (all elements same type).

**Example:**

```python
import numpy as np

# 1D array
arr1 = np.array([1, 2, 3, 4])
print(arr1)       # [1 2 3 4]

# 2D array
arr2 = np.array([[1, 2], [3, 4]])
print(arr2)
# [[1 2]
#  [3 4]]
```

**Array Properties:**

```python
print(arr2.shape)    # (2, 2) => 2 rows, 2 columns
print(arr2.ndim)     # 2 => 2D array
print(arr2.size)     # 4 => total elements
print(arr2.dtype)    # data type
```

---

## **5. NumPy Array Creation Methods**

1. **arange():**
   Python range ke jaisa, lekin array return karta hai.

```python
arr = np.arange(0, 10, 2)
print(arr)   # [0 2 4 6 8]
```

2. **zeros():**
   Specified shape ka array with all zeros.

```python
arr = np.zeros((2,3))
print(arr)
# [[0. 0. 0.]
#  [0. 0. 0.]]
```

3. **ones():**
   Specified shape ka array with all ones.

```python
arr = np.ones((3,2))
print(arr)
```

4. **linspace():**
   Start se end tak **equal intervals** me numbers.

```python
arr = np.linspace(0, 1, 5)
print(arr)   # [0.   0.25 0.5  0.75 1.  ]
```

5. **random numbers:**

```python
arr = np.random.rand(3,3)  # 3x3 array with random numbers between 0 and 1
print(arr)
```

---

## **6. Array Indexing & Slicing**

```python
arr = np.array([10,20,30,40,50])

print(arr[0])    # 10
print(arr[1:4])  # [20 30 40]

# 2D Array
arr2 = np.array([[1,2,3],[4,5,6],[7,8,9]])
print(arr2[0,1]) # 2 => row 0, col 1
print(arr2[:, 1]) # [2 5 8] => 2nd column
```

---

## **7. NumPy Operations**

**a. Arithmetic Operations:**

```python
a = np.array([1,2,3])
b = np.array([4,5,6])

print(a + b)  # [5 7 9]
print(a * b)  # [4 10 18]
print(a - b)  # [-3 -3 -3]
print(a / b)  # [0.25 0.4 0.5]
```

**b. Mathematical Functions:**

```python
arr = np.array([1,4,9])

print(np.sqrt(arr))    # [1. 2. 3.]
print(np.exp(arr))     # e^arr
print(np.log(arr))     # natural log
```

**c. Aggregation Functions:**

```python
arr = np.array([1,2,3,4,5])

print(np.sum(arr))     # 15
print(np.mean(arr))    # 3.0
print(np.max(arr))     # 5
print(np.min(arr))     # 1
print(np.std(arr))     # standard deviation
```

---

## **8. Reshaping & Flattening**

```python
arr = np.arange(1,13)  # [1 2 ... 12]
arr2 = arr.reshape(3,4)
print(arr2)
# [[ 1  2  3  4]
#  [ 5  6  7  8]
#  [ 9 10 11 12]]

# Flatten back to 1D
print(arr2.ravel())  # [1 2 3 ... 12]
```

---

## **9. Advantages over Python List**

| Feature           | Python List   | NumPy Array |
| ----------------- | ------------- | ----------- |
| Speed             | Slow          | Fast        |
| Memory            | High          | Low         |
| Operations        | Loop required | Vectorized  |
| Multi-dimensional | Difficult     | Easy        |

---

## **10. Summary**

* **NumPy** = Python ke liye **fast, efficient numerical library**.
* **ndarray** = NumPy ka core data structure.
* **Vectorized operations** aur **built-in functions** ka use karke calculations fast.
* **Reshaping, indexing, slicing, random numbers** easily possible.
* Machine Learning, Data Science, Scientific Computing me **NumPy indispensable** hai.

---

Agar chaho, main ek **diagram ke saath complete visual guide** bhi bana sakta hoon jo **NumPy ka 1-page cheat sheet** ho jisme sab arrays, operations aur functions dikh rahe ho.

Kya main wo bana doon?


Great! Agar aap **NumPy install karna** chahte ho, toh Python ke liye easiest way hai **pip** use karna. Main step-by-step guide deta hoon:

---

## **1. Check Python Installed**

Terminal/Command Prompt me check karo:

```bash
python --version
```

Ya

```bash
python3 --version
```

Agar version show ho raha hai (e.g., Python 3.11), toh aap ready ho.

---

## **2. Install NumPy using pip**

Terminal/Command Prompt me type karo:

```bash
pip install numpy
```

Ya agar Python 3 ke liye alag command ho:

```bash
pip3 install numpy
```

Ye **latest stable version** install kar dega.

---

## **3. Verify Installation**

Python shell ya IDE me check karo:

```python
import numpy as np
print(np.__version__)
```

Agar version number print ho gaya, matlab installation **successful** hai. ✅

---

## **4. Optional: Upgrade NumPy**

Agar old version hai, upgrade kar sakte ho:

```bash
pip install --upgrade numpy
```

---

Agar chaho, main next step me **NumPy ka pehla simple example run karna** bhi bata doon, jaise array banana aur basic operation karna.

Kya main wo bata doon?


Perfect! Ab hum **NumPy ke basics** cover karenge, step by step **Hinglish me** with examples, taaki aap **first program se start** kar sako.

---

## **1. NumPy Import Karna**

Har program me pehle library import karna padta hai:

```python
import numpy as np
```

* `np` alias use karte hain taaki **code short aur readable** rahe.
* Ye standard practice hai Data Science aur ML me.

---

## **2. NumPy Array (ndarray) Banana**

NumPy ka **core data structure** hai **ndarray** (N-dimensional array).

### **1D Array**

```python
arr = np.array([1, 2, 3, 4, 5])
print(arr)
# Output: [1 2 3 4 5]
print(type(arr))
# Output: <class 'numpy.ndarray'>
```

### **2D Array**

```python
arr2 = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2)
# Output:
# [[1 2 3]
#  [4 5 6]]
```

---

## **3. Array Properties**

```python
print(arr2.shape)   # (2, 3) => 2 rows, 3 columns
print(arr2.ndim)    # 2 => 2D array
print(arr2.size)    # 6 => total elements
print(arr2.dtype)   # datatype, e.g., int64
```

---

## **4. Array Creation Methods**

1. **arange()** – Python ke range jaisa:

```python
arr = np.arange(0, 10, 2)  # 0 to 10, step 2
print(arr)  # [0 2 4 6 8]
```

2. **zeros()** – sab 0 ka array:

```python
arr = np.zeros((2,3))
print(arr)
# [[0. 0. 0.]
#  [0. 0. 0.]]
```

3. **ones()** – sab 1 ka array:

```python
arr = np.ones((3,2))
print(arr)
```

4. **linspace()** – equal intervals me numbers:

```python
arr = np.linspace(0, 1, 5)  
print(arr)  # [0.   0.25 0.5  0.75 1.  ]
```

5. **random()** – random numbers:

```python
arr = np.random.rand(2,3)  # 2x3 array
print(arr)
```

---

## **5. Indexing & Slicing**

### **1D Array**

```python
arr = np.array([10,20,30,40,50])
print(arr[0])     # 10
print(arr[1:4])   # [20 30 40]
```

### **2D Array**

```python
arr2 = np.array([[1,2,3],[4,5,6],[7,8,9]])
print(arr2[0,1])   # 2 (row 0, col 1)
print(arr2[:,1])   # [2 5 8] => 2nd column
print(arr2[1,:])   # [4 5 6] => 2nd row
```

---

## **6. Basic Operations**

### **Arithmetic Operations (Vectorized)**

```python
a = np.array([1,2,3])
b = np.array([4,5,6])

print(a + b)  # [5 7 9]
print(a * b)  # [4 10 18]
print(a - b)  # [-3 -3 -3]
print(a / b)  # [0.25 0.4 0.5]
```

### **Math Functions**

```python
arr = np.array([1,4,9])
print(np.sqrt(arr))  # [1. 2. 3.]
print(np.exp(arr))   # e^arr
print(np.log(arr))   # natural log
```

---

## **7. Aggregation Functions**

```python
arr = np.array([1,2,3,4,5])
print(np.sum(arr))    # 15
print(np.mean(arr))   # 3.0
print(np.max(arr))    # 5
print(np.min(arr))    # 1
print(np.std(arr))    # standard deviation
```

---

## **8. Reshape & Flatten**

```python
arr = np.arange(1,13)         # [1 2 ... 12]
arr2 = arr.reshape(3,4)       # 3 rows, 4 columns
print(arr2)
# [[ 1  2  3  4]
#  [ 5  6  7  8]
#  [ 9 10 11 12]]

print(arr2.ravel())            # Flatten to 1D
```

---

💡 **Tips:**

* NumPy arrays are faster and memory-efficient than Python lists.
* 2D, 3D arrays easily handle matrices and images.
* Machine Learning aur Data Science me NumPy **must-know** hai.

---

Agar chaho, main ab aapke liye **NumPy ka ek mini practice sheet bana doon** jisme **10-15 basic exercises** ho, jisse aap **hands-on practice** kar sako aur concepts strong ho jaye.

Kya main wo bana doon?


Perfect! Ab hum **NumPy arrays create karna** step by step cover karenge, with examples. Ye **basics ke liye sabse important topic** hai.

---

## **1. Python List se NumPy Array Banana**

Sabse simple way hai **Python list** ko **NumPy array** me convert karna.

```python
import numpy as np

# 1D Array
arr1 = np.array([1, 2, 3, 4, 5])
print(arr1)  
# Output: [1 2 3 4 5]

# 2D Array
arr2 = np.array([[1, 2, 3], [4, 5, 6]])
print(arr2)
# Output:
# [[1 2 3]
#  [4 5 6]]
```

**Key Points:**

* NumPy array me **homogeneous data** hota hai (all elements same type).
* Agar list me mixed type ho, NumPy **upcasts** kar deta hai (e.g., int + float → float).

---

## **2. Using `arange()`**

`arange()` Python ke `range()` jaisa hota hai, lekin NumPy array return karta hai.

```python
# 0 se 10 tak, step 2
arr = np.arange(0, 10, 2)
print(arr)  # [0 2 4 6 8]
```

---

## **3. Using `linspace()`**

`linspace(start, end, num)` start se end tak **equal intervals me** numbers generate karta hai.

```python
arr = np.linspace(0, 1, 5)
print(arr)  
# [0.   0.25 0.5  0.75 1.  ]
```

* Useful for plotting graphs or evenly spaced points.

---

## **4. Using `zeros()`**

`zeros(shape)` specified shape ka **array with all zeros** create karta hai.

```python
arr = np.zeros((2,3))
print(arr)
# [[0. 0. 0.]
#  [0. 0. 0.]]
```

---

## **5. Using `ones()`**

`ones(shape)` specified shape ka **array with all ones** create karta hai.

```python
arr = np.ones((3,2))
print(arr)
# [[1. 1.]
#  [1. 1.]
#  [1. 1.]]
```

---

## **6. Using `eye()` (Identity Matrix)**

```python
arr = np.eye(3)  # 3x3 identity matrix
print(arr)
# [[1. 0. 0.]
#  [0. 1. 0.]
#  [0. 0. 1.]]
```

---

## **7. Using `random` Module**

NumPy me **random numbers** generate karna easy hai.

```python
# 0-1 ke beech random numbers
arr = np.random.rand(2,3)
print(arr)

# integers ke liye
arr2 = np.random.randint(1, 10, (2,3))  # 1-9 ke beech
print(arr2)
```

---

## **8. Using `full()`**

`full(shape, fill_value)` ek array banata hai jisme **sab elements same value** ho.

```python
arr = np.full((2,3), 7)
print(arr)
# [[7 7 7]
#  [7 7 7]]
```

---

## **9. Data Type Specify Karna**

NumPy array banate waqt **data type** specify kar sakte ho:

```python
arr = np.array([1, 2, 3], dtype=float)
print(arr)         # [1. 2. 3.]
print(arr.dtype)   # float64
```

---

## ✅ **Summary of Array Creation**

| Function              | Description           |
| --------------------- | --------------------- |
| `np.array()`          | Python list → ndarray |
| `np.arange()`         | Range of numbers      |
| `np.linspace()`       | Evenly spaced numbers |
| `np.zeros()`          | Array of zeros        |
| `np.ones()`           | Array of ones         |
| `np.eye()`            | Identity matrix       |
| `np.random.rand()`    | Random floats         |
| `np.random.randint()` | Random integers       |
| `np.full()`           | Array with same value |

---

Agar chaho, main **ek diagram + visual chart bana doon** jisme **sab array creation methods aur example output** ek hi jagah dikh rahe ho.
Ye **cheat sheet ki tarah** kaam karega.

Kya main wo bana doon?


Perfect! Ab hum **NumPy array indexing aur slicing** ko detail me samjhenge. Ye **arrays ke data ko access aur manipulate karne ka core concept** hai.

---

## **1. 1D Array Indexing**

1D array me elements **single index** se access hote hain, **0 se start** hota hai.

```python id="0j8b3c"
import numpy as np

arr = np.array([10, 20, 30, 40, 50])
print(arr[0])    # 10 => first element
print(arr[3])    # 40 => fourth element
print(arr[-1])   # 50 => last element
print(arr[-2])   # 40 => second last
```

**Tip:** Negative indexing Python list jaisa hi kaam karta hai.

---

## **2. 1D Array Slicing**

Slicing ka syntax:

```text
array[start : end : step]
```

* `start` → starting index (inclusive)
* `end` → ending index (exclusive)
* `step` → interval

```python id="aw0x6r"
arr = np.array([10, 20, 30, 40, 50])

print(arr[1:4])    # [20 30 40] => index 1 to 3
print(arr[:3])     # [10 20 30] => start se 2 tak
print(arr[2:])     # [30 40 50] => index 2 se end tak
print(arr[::2])    # [10 30 50] => step = 2
print(arr[::-1])   # [50 40 30 20 10] => reverse array
```

---

## **3. 2D Array Indexing**

2D array me **row aur column** dono specify karne hote hain:

```python id="ykc1xa"
arr2 = np.array([[1, 2, 3],
                 [4, 5, 6],
                 [7, 8, 9]])

print(arr2[0, 1])   # 2 => first row, second column
print(arr2[2, 0])   # 7 => third row, first column
```

* Syntax: `arr2[row_index, column_index]`

---

## **4. 2D Array Slicing**

```python id="fz4wqv"
arr2 = np.array([[1, 2, 3],
                 [4, 5, 6],
                 [7, 8, 9]])

print(arr2[0:2, 1:3]) 
# [[2 3]
#  [5 6]] => rows 0-1, columns 1-2

print(arr2[:, 1])   
# [2 5 8] => 2nd column (all rows)
print(arr2[1, :])   
# [4 5 6] => 2nd row (all columns)

print(arr2[::2, ::2])
# [[1 3]
#  [7 9]] => step = 2 for rows & columns
```

**Tip:**

* `:` ka matlab **“all”**
* `::step` ka matlab **skip elements**

---

## **5. Boolean Indexing (Advanced)**

Array me **condition apply karke elements select karna**:

```python id="xbvfr2"
arr = np.array([10, 15, 20, 25, 30])

print(arr[arr > 20])   # [25 30] => elements greater than 20
print(arr[arr % 2 == 0])  # [10 20 30] => even numbers
```

2D arrays me bhi kaam karta hai:

```python id="n0d72q"
arr2 = np.array([[1, 2, 3],
                 [4, 5, 6]])

print(arr2[arr2 > 3])
# [4 5 6]
```

---

## **6. Modifying Array Elements using Indexing & Slicing**

```python id="2gjt2c"
arr = np.array([10, 20, 30, 40, 50])

arr[0] = 99
print(arr)  # [99 20 30 40 50]

arr[1:4] = 100
print(arr)  # [ 99 100 100 100 50]
```

2D array me bhi modify kar sakte ho:

```python id="kd4rpy"
arr2 = np.array([[1, 2, 3], [4, 5, 6]])
arr2[0, :] = 9
print(arr2)
# [[9 9 9]
#  [4 5 6]]
```

---

## ✅ **Summary Table**

| Concept        | Syntax / Example | Meaning            |
| -------------- | ---------------- | ------------------ |
| 1D Index       | `arr[0]`         | First element      |
| 1D Slice       | `arr[1:4]`       | Index 1 to 3       |
| Negative Index | `arr[-1]`        | Last element       |
| 2D Index       | `arr2[0,1]`      | Row 0, Col 1       |
| 2D Slice       | `arr2[0:2, 1:3]` | Rows 0-1, Cols 1-2 |
| All Rows/Cols  | `arr2[:,1]`      | 2nd column         |
| Step           | `arr[::2]`       | Every 2nd element  |
| Boolean Index  | `arr[arr>20]`    | Elements >20       |

---

💡 **Tip:**

* Indexing aur slicing me **original array ka reference hota hai**, matlab change directly affect karega original array ko.

---

Agar chaho, main next me **NumPy Advanced Indexing Tricks** aur **Fancy Indexing with Examples** bhi bata doon jo **real-world data manipulation me bohot useful** hai.

Kya main wo bata doon?


Perfect! Ab hum **NumPy arrays ko reshape aur resize karna** detail me samjhenge. Ye **array manipulation ke core concepts** hai, especially **ML aur data processing me**.

---

## **1. Reshaping Arrays**

**Reshape** se hum array ka **shape change** kar sakte hain **without changing elements**.

**Syntax:**

```python
new_array = array.reshape(new_shape)
```

* Total elements **same** hone chahiye (`old_size == new_size`)
* N-dimensional arrays me bhi kaam karta hai

### **Example 1: 1D → 2D**

```python id="v2k1h5"
import numpy as np

arr = np.arange(1, 13)  # [1 2 ... 12]
print("Original array:", arr)

arr2 = arr.reshape(3, 4)  # 3 rows, 4 columns
print("Reshaped 2D array:\n", arr2)
```

**Output:**

```
Original array: [ 1  2  3  4  5  6  7  8  9 10 11 12]
Reshaped 2D array:
 [[ 1  2  3  4]
  [ 5  6  7  8]
  [ 9 10 11 12]]
```

---

### **Example 2: 2D → 3D**

```python id="j4kgp9"
arr3d = arr2.reshape(2, 2, 3)  # 2 blocks, 2 rows, 3 columns
print(arr3d)
```

**Output:**

```
[[[ 1  2  3]
  [ 4  5  6]]

 [[ 7  8  9]
  [10 11 12]]]
```

**Tip:**

* `-1` use kar ke **auto-calculate dimension** kar sakte ho:

```python id="lq0sfr"
arr2 = arr.reshape(2, -1)  # 2 rows, 6 columns auto
print(arr2)
```

---

## **2. Flatten / Ravel Array**

**Flatten** ka matlab **multi-dimensional array ko 1D me convert karna**.

```python id="9m2s4q"
arr_flat = arr2.ravel()  # returns a flattened 1D array
print(arr_flat)
# [ 1  2  3  4  5  6  7  8  9 10 11 12]
```

* Difference: `ravel()` → **view (original array affect hota hai)**
* `flatten()` → **copy (original array safe)**

```python id="6x1phn"
arr_flat2 = arr2.flatten()
```

---

## **3. Resizing Arrays**

**Resize** se array ka **shape permanently change** ho jata hai.

```python id="c3uw7x"
arr = np.array([1, 2, 3, 4, 5, 6])
arr.resize((3,2))
print(arr)
# [[1 2]
#  [3 4]
#  [5 6]]
```

* Agar new size **bada hai**, extra elements **0 se fill** honge
* Agar **chhota**, elements **truncate** ho jayenge

```python id="a1m2fr"
arr.resize((2,5))
print(arr)
# [[1 2 3 4 5]
#  [6 0 0 0 0]]
```

**Tip:**

* `reshape()` → returns **new array**
* `resize()` → modifies **original array**

---

## **4. Transpose an Array**

Transpose = rows ↔ columns swap

```python id="9oqfiv"
arr2 = np.array([[1,2,3],[4,5,6]])
print("Original:\n", arr2)

arr_T = arr2.T
print("Transposed:\n", arr_T)
```

**Output:**

```
Original:
 [[1 2 3]
  [4 5 6]]
Transposed:
 [[1 4]
  [2 5]
  [3 6]]
```

---

## **5. Summary Table**

| Operation | Syntax                          | Description                             |
| --------- | ------------------------------- | --------------------------------------- |
| Reshape   | `arr.reshape(new_shape)`        | Return new array with shape             |
| Flatten   | `arr.ravel()` / `arr.flatten()` | Multi-D → 1D                            |
| Resize    | `arr.resize(new_shape)`         | Change original array shape permanently |
| Transpose | `arr.T`                         | Swap rows & columns                     |

---

💡 **Important Notes:**

1. `reshape()` **original array affect nahi karta**
2. `resize()` **original array modify karta hai**
3. `-1` dimension **auto calculate** ke liye use hota hai

---

Agar chaho, main **ek visual diagram + example table** bana doon jisme **Reshape, Flatten, Resize aur Transpose** ek hi jagah dikh rahe ho, jisse ye **NumPy array manipulation cheat sheet** ban jaye.

Kya main wo bana doon?


Perfect! Ab hum **NumPy me arrays ko stack aur split karna** detail me samjhenge. Ye **data manipulation ke liye bohot important concepts** hain, especially **ML aur data processing me**.

---

## **1. Stacking Arrays**

**Stacking** ka matlab hai **do ya zyada arrays ko join karna**. NumPy me alag-alag types ke stacking hain: **vertical, horizontal, column-wise, row-wise**.

---

### **1.1 Horizontal Stacking (`hstack`)**

Arrays ko **side by side (columns me)** join karta hai.

```python id="5j0kxl"
import numpy as np

a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

arr_h = np.hstack((a, b))
print(arr_h)
# Output: [1 2 3 4 5 6]
```

2D arrays me:

```python id="g0l4xr"
a2 = np.array([[1,2],[3,4]])
b2 = np.array([[5,6],[7,8]])

arr_h2 = np.hstack((a2, b2))
print(arr_h2)
# [[1 2 5 6]
#  [3 4 7 8]]
```

---

### **1.2 Vertical Stacking (`vstack`)**

Arrays ko **top-bottom (rows me)** join karta hai.

```python id="h3m2wl"
arr_v = np.vstack((a, b))
print(arr_v)
# [[1 2 3]
#  [4 5 6]]
```

2D arrays me:

```python id="r1p9xo"
arr_v2 = np.vstack((a2, b2))
print(arr_v2)
# [[1 2]
#  [3 4]
#  [5 6]
#  [7 8]]
```

---

### **1.3 Column Stacking (`column_stack`)**

1D arrays ko **columns me merge** karta hai (jaise 2D matrix).

```python id="t8q5mw"
arr_col = np.column_stack((a, b))
print(arr_col)
# [[1 4]
#  [2 5]
#  [3 6]]
```

---

### **1.4 Row Stacking (`row_stack`)**

`row_stack()` almost **vstack** ke jaisa hi kaam karta hai.

```python id="u9y2pb"
arr_row = np.row_stack((a, b))
print(arr_row)
# [[1 2 3]
#  [4 5 6]]
```

---

## **2. Splitting Arrays**

**Splitting** ka matlab hai **array ko multiple arrays me divide karna**. NumPy me:

* `hsplit` → horizontal split (columns ke according)
* `vsplit` → vertical split (rows ke according)
* `split` → general split

---

### **2.1 Horizontal Split (`hsplit`)**

```python id="s6k7uv"
arr = np.array([[1,2,3,4],[5,6,7,8]])
arr_hsplit = np.hsplit(arr, 2)  # 2 parts
print(arr_hsplit)
# [array([[1, 2],
#         [5, 6]]), 
#  array([[3, 4],
#         [7, 8]])]
```

---

### **2.2 Vertical Split (`vsplit`)**

```python id="p4r3xz"
arr_vsplit = np.vsplit(arr, 2)  # 2 parts
print(arr_vsplit)
# [array([[1, 2, 3, 4]]), 
#  array([[5, 6, 7, 8]])]
```

---

### **2.3 General Split (`split`)**

1D array ko **equal parts me divide** karne ke liye:

```python id="m9q1yk"
arr1d = np.array([1,2,3,4,5,6])
arr_split = np.split(arr1d, 3)  # 3 equal parts
print(arr_split)
# [array([1, 2]), array([3, 4]), array([5, 6])]
```

**Note:** Total elements divisible by number of splits hona chahiye, warna error aayega.

---

## **3. Summary Table**

| Operation        | Function                 | Example             |
| ---------------- | ------------------------ | ------------------- |
| Horizontal Stack | `np.hstack((a,b))`       | Side by side join   |
| Vertical Stack   | `np.vstack((a,b))`       | Top-bottom join     |
| Column Stack     | `np.column_stack((a,b))` | Columns merge 1D→2D |
| Row Stack        | `np.row_stack((a,b))`    | Rows merge 1D→2D    |
| Horizontal Split | `np.hsplit(arr, n)`      | Split columns       |
| Vertical Split   | `np.vsplit(arr, n)`      | Split rows          |
| General Split    | `np.split(arr, n)`       | 1D array split      |

---

💡 **Tips:**

1. **Stacking** → arrays ko **merge** karna
2. **Splitting** → array ko **divide** karna
3. Horizontal vs Vertical → **columns vs rows**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme stacking & splitting ka diagram ho** jisse **arrays merge aur split kaise hote hain** clearly samajh aaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy Broadcasting** ko detail me samjhenge. Ye concept **arrays ke size different hone par bhi operations allow karne ke liye** bohot important hai.

---

## **1. Broadcasting kya hai?**

**Broadcasting** ka matlab hai **do arrays with different shapes ko automatically compatible bana ke operations perform karna**.

* NumPy **smaller array ko automatically expand** karta hai taaki **shape match ho jaye**.
* Ye **loops ke bina vectorized operations** possible banata hai.

---

### **Rule of Broadcasting**

1. Agar **number of dimensions different hai**, smaller array me **1s add** kar diye jate hain left side me.
2. Arrays ke **dimensions last se match hone chahiye** ya **1 hona chahiye**.
3. Agar **match nahi hota**, error aata hai.

---

## **2. Example 1: 1D + 1D**

```python id="x3b9s0"
import numpy as np

a = np.array([1, 2, 3])
b = np.array([4, 5, 6])

print(a + b)
# Output: [5 7 9]
```

* Shapes same hai `[3]`, simple element-wise addition.

---

## **3. Example 2: 2D + 1D (Row Vector)**

```python id="q8f2cl"
a = np.array([[1,2,3],
              [4,5,6]])
b = np.array([10,20,30])

print(a + b)
```

**Output:**

```id="5yq0zx"
[[11 22 33]
 [14 25 36]]
```

* Smaller array `[10,20,30]` **row-wise broadcast** ho gaya.

---

## **4. Example 3: 2D + 1D (Column Vector)**

```python id="k2w5bq"
a = np.array([[1,2,3],
              [4,5,6]])
b = np.array([[10],
              [20]])

print(a + b)
```

**Output:**

```id="u8g9ry"
[[11 12 13]
 [24 25 26]]
```

* Smaller array `[10],[20]` **column-wise broadcast** ho gaya.

---

## **5. Example 4: Scalar + Array**

```python id="j9p3la"
arr = np.array([1,2,3,4])
print(arr + 5)
# Output: [6 7 8 9]
```

* Scalar automatically **broadcast** ho gaya pure array ke across.

---

## **6. Shapes Compatibility**

| Array A Shape | Array B Shape | Compatible? | Result Shape |
| ------------- | ------------- | ----------- | ------------ |
| (3,4)         | (4,)          | Yes         | (3,4)        |
| (3,4)         | (3,1)         | Yes         | (3,4)        |
| (3,4)         | (2,4)         | No          | Error        |
| (5,1,3)       | (1,4,3)       | Yes         | (5,4,3)      |

---

## **7. Practical Use in ML / Data Science**

1. Normalize data:

```python id="l7p1vx"
X = np.array([[1,2,3],[4,5,6]])
mean = np.mean(X, axis=0)    # [2.5 3.5 4.5]
X_norm = X - mean
print(X_norm)
# [[-1.5 -1.5 -1.5]
#  [ 1.5  1.5  1.5]]
```

* Broadcasting automatically **mean subtract** karta hai har row se.

2. Adding bias vector in neural networks:

```python id="p5v9cq"
Z = np.array([[0.1,0.2,0.3],
              [0.4,0.5,0.6]])
b = np.array([0.01,0.02,0.03])
Z_new = Z + b
```

* Bias vector automatically **broadcast** ho gaya har row me.

---

## **8. Summary**

| Concept        | Explanation                                                             |
| -------------- | ----------------------------------------------------------------------- |
| Broadcasting   | Automatic expansion of arrays for element-wise operations               |
| Rules          | 1. Add 1s to smaller array dims, 2. Last dims match or 1, 3. Else error |
| Scalar + Array | Scalar broadcast over all elements                                      |
| 1D + 2D        | Row/column vector expanded automatically                                |
| Practical Use  | Data normalization, adding bias, vectorized computations                |

---

💡 **Tip:** Broadcasting se **loops avoid hote hain**, operations **fast ho jate hain**, aur **code concise aur readable** ban jata hai.

---

Agar chaho, main **Broadcasting ka ek visual diagram bana doon** jisme **different shapes ke arrays aur unka broadcast result** dikh raha ho.
Ye **concept samajhne me bohot helpful** hoga.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy ke basic arithmetic operations** detail me samjhenge. Ye **arrays pe calculations karne ka core concept** hai aur ML/data science me bohot use hota hai.

---

## **1. NumPy Arrays for Arithmetic**

NumPy me **arithmetic operations element-wise** hoti hain, matlab **har element individually compute** hota hai.

```python id="w8l7kp"
import numpy as np

a = np.array([10, 20, 30, 40])
b = np.array([1, 2, 3, 4])
```

---

## **2. Addition**

```python id="k2m8vz"
c = a + b
print(c)
# Output: [11 22 33 44]
```

* **Element-wise addition**
* Python list ke comparison me bohot fast hai

---

## **3. Subtraction**

```python id="p3n9fq"
c = a - b
print(c)
# Output: [9 18 27 36]
```

---

## **4. Multiplication**

```python id="x4q1kp"
c = a * b
print(c)
# Output: [10 40 90 160]
```

* Element-wise multiply hota hai
* **Matrix multiplication** ke liye `@` operator ya `np.dot()` use hota hai

---

## **5. Division**

```python id="r6t3lm"
c = a / b
print(c)
# Output: [10. 10. 10. 10.]
```

* Element-wise division
* Result **float array** me hota hai

```python id="s7y4nn"
c = a // b   # Floor division
print(c)
# Output: [10 10 10 10]
```

---

## **6. Modulus (Remainder)**

```python id="t8u5op"
c = a % b
print(c)
# Output: [0 0 0 0]
```

---

## **7. Exponentiation**

```python id="v9w6qr"
c = a ** 2
print(c)
# Output: [100 400 900 1600]

# Element-wise power
c = a ** b
print(c)
# Output: [10 400 27000 256000]
```

---

## **8. Using NumPy Math Functions**

NumPy me **built-in mathematical functions** ka use bhi kar sakte hain:

```python id="y1x7st"
arr = np.array([1,4,9,16])

print(np.sqrt(arr))   # [1. 2. 3. 4.] → Square root
print(np.exp(arr))    # e^arr
print(np.log(arr))    # Natural log
print(np.sin(arr))    # Trigonometric function
```

---

## **9. Aggregation Functions (Arithmetic on whole array)**

```python id="z2y8uv"
arr = np.array([1,2,3,4,5])

print(np.sum(arr))     # 15 → sum of elements
print(np.mean(arr))    # 3.0 → average
print(np.min(arr))     # 1 → minimum
print(np.max(arr))     # 5 → maximum
print(np.prod(arr))    # 120 → product of elements
```

---

## **10. Broadcasting with Arithmetic Operations**

```python id="a3b9cd"
a = np.array([1,2,3])
b = 10
print(a + b)  # [11 12 13] → Scalar broadcast
```

* **Smaller array/scalar** automatically **expanded** to match shape

---

## **11. Summary Table**

| Operation      | Symbol / Function | Example        | Output          |
| -------------- | ----------------- | -------------- | --------------- |
| Addition       | `+`               | `[1,2]+[3,4]`  | `[4,6]`         |
| Subtraction    | `-`               | `[5,6]-[1,2]`  | `[4,4]`         |
| Multiplication | `*`               | `[1,2]*[3,4]`  | `[3,8]`         |
| Division       | `/`               | `[4,6]/[2,3]`  | `[2.,2.]`       |
| Floor Division | `//`              | `[5,6]//[2,3]` | `[2,2]`         |
| Modulus        | `%`               | `[5,6]%[2,3]`  | `[1,0]`         |
| Power          | `**`              | `[2,3]**2`     | `[4,9]`         |
| Square Root    | `np.sqrt()`       | `[1,4,9]`      | `[1.,2.,3.]`    |
| Exponential    | `np.exp()`        | `[1,2]`        | `[2.718,7.389]` |

---

💡 **Tips:**

1. Arithmetic operations **vectorized** → **loops avoid hote hain**
2. Broadcasting ke saath **different shapes ke arrays** bhi compute kar sakte ho
3. ML aur scientific computing me ye operations **fast aur efficient** hain

---

Agar chaho, main **ek visual cheat sheet** bana doon jisme **addition, subtraction, multiplication, division, power, sqrt, exp, log** sab ek hi diagram me **example + output** dikh raha ho.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy ke aggregation functions** detail me samjhenge. Ye **arrays ke upar calculations karne ke liye bohot important** hain, specially **data analysis aur ML me**.

---

## **1. Aggregation Functions kya hai?**

Aggregation functions **ek array ke multiple elements ko ek single value me summarize** karte hain.
NumPy me common functions hain:

* `sum()` → total sum
* `mean()` → average
* `max()` → maximum value
* `min()` → minimum value

---

## **2. Example Array**

```python id="b2n7la"
import numpy as np

arr = np.array([10, 20, 30, 40, 50])
print("Array:", arr)
```

---

## **3. Sum**

```python id="k3p8qd"
total = np.sum(arr)
print("Sum:", total)
# Output: Sum: 150
```

* 2D array me row/column wise sum bhi kar sakte ho:

```python id="m1q9vz"
arr2d = np.array([[1,2,3],[4,5,6]])
print("Sum all elements:", np.sum(arr2d))           # 21
print("Sum of columns:", np.sum(arr2d, axis=0))     # [5 7 9]
print("Sum of rows:", np.sum(arr2d, axis=1))        # [6 15]
```

**Tip:** `axis=0` → columns, `axis=1` → rows

---

## **4. Mean (Average)**

```python id="p4r7kw"
avg = np.mean(arr)
print("Mean:", avg)
# Output: Mean: 30.0

# 2D Array
print("Mean of columns:", np.mean(arr2d, axis=0))   # [2.5 3.5 4.5]
print("Mean of rows:", np.mean(arr2d, axis=1))      # [2. 5.]
```

---

## **5. Max**

```python id="s5t9mz"
maximum = np.max(arr)
print("Max:", maximum)  
# Output: Max: 50

# 2D array
print("Max of columns:", np.max(arr2d, axis=0))     # [4 5 6]
print("Max of rows:", np.max(arr2d, axis=1))        # [3 6]
```

---

## **6. Min**

```python id="t6u0nc"
minimum = np.min(arr)
print("Min:", minimum)  
# Output: Min: 10

# 2D array
print("Min of columns:", np.min(arr2d, axis=0))     # [1 2 3]
print("Min of rows:", np.min(arr2d, axis=1))        # [1 4]
```

---

## **7. Summary Table**

| Function    | Description             | Example Output |
| ----------- | ----------------------- | -------------- |
| `np.sum()`  | Sum of all elements     | 150            |
| `np.mean()` | Average (mean)          | 30.0           |
| `np.max()`  | Maximum value           | 50             |
| `np.min()`  | Minimum value           | 10             |
| Axis=0      | Column-wise aggregation | [5 7 9]        |
| Axis=1      | Row-wise aggregation    | [6 15]         |

---

💡 **Tips:**

1. **axis parameter** ka use karke rows ya columns pe operation kar sakte ho.
2. Ye aggregation functions **fast and vectorized** hain, loops ki zarurat nahi.
3. Data analysis, statistics aur ML me ye **data summarize karne ke liye** bohot important hai.

---

Agar chaho, main ek **visual cheat sheet bana doon jisme sum, mean, max, min ka 1D & 2D example + output** diagram me dikh raha ho, jisse concept **instant samajh aaye**.

Chahte ho main wo bana doon?



Perfect! Ab hum **NumPy Universal Functions (ufuncs)** ko detail me samjhenge. Ye concept **arrays pe fast element-wise computations** ke liye bohot important hai.

---

## **1. Universal Functions (ufuncs) kya hai?**

**Universal Functions (ufuncs)** NumPy ke **built-in functions** hote hain jo **element-wise operations** perform karte hain:

* Fast and vectorized
* Array ke **har element pe individually apply** hote hain
* Mathematical, trigonometric, logarithmic, exponential operations ke liye use hote hain

---

## **2. Mathematical ufuncs**

### **2.1 Square Root**

```python id="s1t9pl"
import numpy as np

arr = np.array([1, 4, 9, 16])
print(np.sqrt(arr))
# Output: [1. 2. 3. 4.]
```

### **2.2 Exponential**

```python id="p3r8kn"
arr = np.array([1, 2, 3])
print(np.exp(arr))
# Output: [ 2.71828183  7.3890561  20.08553692]
```

### **2.3 Logarithm**

```python id="v5q1lz"
arr = np.array([1, np.e, np.e**2])
print(np.log(arr))
# Output: [0. 1. 2.]
```

### **2.4 Absolute Value**

```python id="k8w2ma"
arr = np.array([-1, -5, 3])
print(np.abs(arr))
# Output: [1 5 3]
```

---

## **3. Trigonometric ufuncs**

```python id="x9p3bn"
angles = np.array([0, np.pi/2, np.pi])

print(np.sin(angles))  # [0. 1. 0.]
print(np.cos(angles))  # [1. 0. -1.]
print(np.tan(angles))  # [0. 1.63312394e+16 -0.]
```

* All operations **element-wise** hoti hain
* Angles **radians** me dena zaruri hai

---

## **4. Rounding Functions**

```python id="y2q5lc"
arr = np.array([1.2, 2.5, 3.7, 4.0])

print(np.floor(arr))   # [1. 2. 3. 4.] → round down
print(np.ceil(arr))    # [2. 3. 4. 4.] → round up
print(np.round(arr))   # [1. 2. 4. 4.] → nearest integer
```

---

## **5. Binary ufuncs (Two arrays)**

NumPy me **2 arrays pe element-wise operation**:

```python id="z3s6ma"
a = np.array([1,2,3])
b = np.array([4,5,6])

print(np.add(a, b))    # [5 7 9]
print(np.subtract(a, b)) # [-3 -3 -3]
print(np.multiply(a, b)) # [ 4 10 18]
print(np.divide(a, b))   # [0.25 0.4 0.5]
print(np.maximum(a, b))  # [4 5 6]
print(np.minimum(a, b))  # [1 2 3]
```

* Binary ufuncs me **2 arrays ka shape broadcasting rules follow karega**

---

## **6. Comparison ufuncs**

Element-wise **logical comparison**:

```python id="a4q7mz"
a = np.array([1,2,3])
b = np.array([2,2,2])

print(np.equal(a, b))    # [False  True False]
print(np.not_equal(a,b))  # [ True False  True]
print(np.greater(a,b))    # [False False  True]
print(np.less_equal(a,b)) # [ True  True False]
```

---

## **7. Summary Table**

| Type                 | Function Example                                    | Description             |
| -------------------- | --------------------------------------------------- | ----------------------- |
| Mathematical         | `np.sqrt`, `np.exp`, `np.log`                       | Element-wise math       |
| Trigonometric        | `np.sin`, `np.cos`, `np.tan`                        | Angles in radians       |
| Rounding             | `np.floor`, `np.ceil`, `np.round`                   | Round elements          |
| Binary               | `np.add`, `np.subtract`, `np.multiply`, `np.divide` | 2-array operations      |
| Comparison / Logical | `np.equal`, `np.greater`, `np.less_equal`           | Element-wise comparison |
| Absolute             | `np.abs`                                            | Element-wise absolute   |

---

💡 **Tips:**

1. Universal functions **loops avoid karte hain**, fast vectorized operations provide karte hain.
2. **Broadcasting rules** follow karke different shaped arrays pe bhi kaam karte hain.
3. ML, DL, aur scientific computing me **ufuncs sabse commonly used tools** hain.

---

Agar chaho, main **ek visual chart bana doon jisme common ufuncs + example output** dikh rahe ho jisse **quick reference cheat sheet** ban jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy ke Mathematical Functions** detail me samjhenge. Ye **arrays pe fast, element-wise mathematical operations** ke liye bohot important hai, especially **data science aur machine learning me**.

---

## **1. Common Mathematical Functions in NumPy**

NumPy me **built-in mathematical functions** (ufuncs) available hain. Ye **element-wise operations** perform karte hain:

---

### **1.1 Absolute Value (`np.abs`)**

```python id="a1b9mz"
import numpy as np

arr = np.array([-1, -5, 3, -7])
print(np.abs(arr))
# Output: [1 5 3 7]
```

* Negative numbers ko positive me convert karta hai

---

### **1.2 Square Root (`np.sqrt`)**

```python id="c2d8pq"
arr = np.array([1, 4, 9, 16])
print(np.sqrt(arr))
# Output: [1. 2. 3. 4.]
```

* Element-wise square root calculate karta hai

---

### **1.3 Power (`np.power`)**

```python id="e3f7rx"
arr = np.array([2, 3, 4])
print(np.power(arr, 2))   # Square each element
# Output: [4 9 16]

print(np.power(arr, 3))   # Cube each element
# Output: [ 8 27 64]
```

---

### **1.4 Exponential (`np.exp`)**

```python id="g4h6sa"
arr = np.array([1, 2, 3])
print(np.exp(arr))
# Output: [ 2.71828183  7.3890561  20.08553692] (e^arr)
```

* e^x calculate karta hai (natural exponent)

---

### **1.5 Logarithm**

```python id="i5j5tb"
arr = np.array([1, np.e, np.e**2])
print(np.log(arr))
# Output: [0. 1. 2.] → natural log (ln)

print(np.log10([1, 10, 100])) 
# Output: [0. 1. 2.] → base-10 log
```

* `np.log()` → natural log (base e)
* `np.log10()` → log base 10

---

### **1.6 Trigonometric Functions**

Angles **radians me dena hota hai**:

```python id="k6l4uc"
angles = np.array([0, np.pi/2, np.pi])

print(np.sin(angles))  # [0. 1. 0.]
print(np.cos(angles))  # [1. 0. -1.]
print(np.tan(angles))  # [0. 1.63312394e+16 -0.]
```

* Inverse trigonometric: `np.arcsin()`, `np.arccos()`, `np.arctan()`

---

### **1.7 Rounding Functions**

```python id="m7n3vd"
arr = np.array([1.2, 2.5, 3.7, 4.0])

print(np.floor(arr))  # Round down → [1. 2. 3. 4.]
print(np.ceil(arr))   # Round up   → [2. 3. 4. 4.]
print(np.round(arr))  # Round nearest → [1. 2. 4. 4.]
```

---

### **1.8 Other Useful Functions**

| Function                     | Description                      |
| ---------------------------- | -------------------------------- |
| `np.sum(arr)`                | Sum of elements                  |
| `np.prod(arr)`               | Product of elements              |
| `np.mean(arr)`               | Average (mean)                   |
| `np.std(arr)`                | Standard deviation               |
| `np.var(arr)`                | Variance                         |
| `np.min(arr)`                | Minimum value                    |
| `np.max(arr)`                | Maximum value                    |
| `np.clip(arr, a_min, a_max)` | Limit values between min and max |

```python id="o8p2we"
arr = np.array([1, 5, 10, 15])
print(np.clip(arr, 3, 12))  # [3 5 10 12]
```

---

## **2. Broadcasting with Math Functions**

Math functions **broadcasting ke saath kaam karte hain**:

```python id="q9r1xy"
arr = np.array([[1,2,3],[4,5,6]])
print(np.sqrt(arr))  
# [[1.         1.41421356 1.73205081]
#  [2.         2.23606798 2.44948974]]
```

* Scalar ya smaller array ke saath bhi operations possible hain

---

## **3. Summary Table**

| Function     | Example                 | Output Example  |
| ------------ | ----------------------- | --------------- |
| `np.abs()`   | `np.abs([-2,3])`        | `[2,3]`         |
| `np.sqrt()`  | `np.sqrt([4,9])`        | `[2,3]`         |
| `np.power()` | `np.power([2,3],2)`     | `[4,9]`         |
| `np.exp()`   | `np.exp([1,2])`         | `[2.718,7.389]` |
| `np.log()`   | `np.log([1,np.e])`      | `[0,1]`         |
| `np.sin()`   | `np.sin([0,np.pi/2])`   | `[0,1]`         |
| `np.floor()` | `np.floor([1.7,2.3])`   | `[1,2]`         |
| `np.ceil()`  | `np.ceil([1.7,2.3])`    | `[2,3]`         |
| `np.round()` | `np.round([1.5,2.3])`   | `[2,2]`         |
| `np.clip()`  | `np.clip([1,5,10],3,8)` | `[3,5,8]`       |

---

💡 **Tips:**

1. NumPy mathematical functions **element-wise** aur **vectorized** hote hain → loops avoid hote hain.
2. Broadcasting ke saath **different shaped arrays** pe bhi operations possible hain.
3. ML, DL aur scientific computing me **fast calculations ke liye must-know** functions hain.

---

Agar chaho, main **ek visual cheat sheet bana doon jisme common mathematical functions + example output** diagram me dikh raha ho jisse **quick reference** ban jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Matrix Multiplication aur Manipulation** detail me samjhenge. Ye **linear algebra aur machine learning ke liye core concepts** hain.

---

## **1. Matrix Multiplication**

NumPy me **element-wise multiplication aur true matrix multiplication** alag hote hain.

---

### **1.1 Element-wise Multiplication (`*`)**

```python id="a1b2c3"
import numpy as np

A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

C = A * B
print(C)
# Output:
# [[ 5 12]
#  [21 32]]
```

* Har element **corresponding element se multiply** hota hai
* Isko **Hadamard product** bhi kehte hain

---

### **1.2 Matrix Multiplication (`@` or `np.dot`)**

```python id="d4e5f6"
C = A @ B
print(C)
# Output:
# [[19 22]
#  [43 50]]

# Same using np.dot
C2 = np.dot(A, B)
print(C2)
# [[19 22]
#  [43 50]]
```

**Rule:** Number of **columns in first matrix = number of rows in second matrix**

---

## **2. Transpose**

Transpose ka matlab hai **rows aur columns swap karna**:

```python id="g7h8i9"
A_T = A.T
print(A_T)
# [[1 3]
#  [2 4]]
```

* Useful in matrix multiplication, linear algebra, ML

---

## **3. Inverse of a Matrix**

Square matrix ka **inverse** `np.linalg.inv()` se nikalte hain:

```python id="j1k2l3"
A = np.array([[1,2],[3,4]])
A_inv = np.linalg.inv(A)
print(A_inv)
# [[-2.   1. ]
#  [ 1.5 -0.5]]
```

* Multiplying matrix with its inverse → **identity matrix**

```python id="m4n5o6"
I = A @ A_inv
print(np.round(I, 2))
# [[1. 0.]
#  [0. 1.]]
```

---

## **4. Determinant**

Matrix ka **determinant** `np.linalg.det()` se nikalte hain:

```python id="p7q8r9"
det = np.linalg.det(A)
print(det)
# -2.0
```

* Determinant = 0 → matrix singular, inverse nahi hota

---

## **5. Eigenvalues and Eigenvectors**

```python id="s1t2u3"
eigvals, eigvecs = np.linalg.eig(A)
print("Eigenvalues:", eigvals)
print("Eigenvectors:\n", eigvecs)
```

* ML aur PCA me **dimensionality reduction** ke liye use hota hai

---

## **6. Identity & Diagonal Matrices**

```python id="v4w5x6"
I = np.eye(3)  # 3x3 identity matrix
print(I)
# [[1. 0. 0.]
#  [0. 1. 0.]
#  [0. 0. 1.]]

diag = np.diag([10,20,30])
print(diag)
# [[10  0  0]
#  [ 0 20  0]
#  [ 0  0 30]]
```

---

## **7. Flatten, Reshape, Resize with Matrices**

```python id="y7z8a9"
A = np.array([[1,2,3],[4,5,6]])

flat = A.flatten()
print(flat)  # [1 2 3 4 5 6]

reshape = A.reshape(3,2)
print(reshape)
# [[1 2]
#  [3 4]
#  [5 6]]
```

* Useful in **data preprocessing** for ML

---

## **8. Summary Table**

| Operation                   | Function / Syntax        | Example / Output    |
| --------------------------- | ------------------------ | ------------------- |
| Element-wise multiplication | `A * B`                  | [[5 12],[21 32]]    |
| Matrix multiplication       | `A @ B` or `np.dot(A,B)` | [[19 22],[43 50]]   |
| Transpose                   | `A.T`                    | [[1 3],[2 4]]       |
| Inverse                     | `np.linalg.inv(A)`       | [[-2 1],[1.5 -0.5]] |
| Determinant                 | `np.linalg.det(A)`       | -2.0                |
| Eigenvalues/Eigenvectors    | `np.linalg.eig(A)`       | array, matrix       |
| Identity matrix             | `np.eye(n)`              | 1s diagonal         |
| Diagonal matrix             | `np.diag([a,b,c])`       | diagonal values     |
| Flatten                     | `A.flatten()`            | 1D array            |
| Reshape                     | `A.reshape(rows, cols)`  | new shape           |

---

💡 **Tips:**

1. `*` → element-wise, `@` → matrix multiplication
2. **Linear algebra functions** → `np.linalg` module me
3. ML, DL, PCA, Regression me **matrix multiplication aur inverse** frequently use hota hai

---

Agar chaho, main **ek visual cheat sheet bana doon jisme matrix multiplication, transpose, inverse, determinant aur flatten/reshape sab ek diagram me dikh rahe ho**.
Ye **quick reference aur concept clarity ke liye bohot useful** hoga.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Matrix aur Vector Products** ko detail me samjhenge. Ye **linear algebra aur ML ke liye core concepts** hain.

---

## **1. Vector Dot Product**

**Dot product (scalar product)** = 2 vectors ka **sum of products of corresponding elements**.

```python id="v1a2b3"
import numpy as np

v1 = np.array([1,2,3])
v2 = np.array([4,5,6])

dot = np.dot(v1, v2)
print(dot)
# Output: 1*4 + 2*5 + 3*6 = 32
```

* NumPy me `np.dot()` ya `@` operator dono kaam karte hain:

```python id="v1c2d3"
dot2 = v1 @ v2
print(dot2)  # 32
```

---

## **2. Vector Cross Product**

**Cross product** = 3D vectors ka **vector perpendicular to both**.

```python id="v2e3f4"
v1 = np.array([1,2,3])
v2 = np.array([4,5,6])

cross = np.cross(v1, v2)
print(cross)
# Output: [-3  6 -3]
```

* Useful in **physics, 3D graphics, rotations**

---

## **3. Matrix-Vector Product**

Matrix × Vector → Result **vector**:

```python id="v3g4h5"
A = np.array([[1,2,3],[4,5,6]])
v = np.array([1,0,1])

result = A @ v
print(result)
# Output: [1*1+2*0+3*1, 4*1+5*0+6*1] = [4 10]
```

* NumPy me `@` ya `np.dot()` use hota hai

---

## **4. Matrix-Matrix Product**

```python id="v4i5j6"
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

C = A @ B
print(C)
# [[1*5+2*7, 1*6+2*8], [3*5+4*7, 3*6+4*8]]
# Output: [[19 22]
#          [43 50]]
```

* **Rule:** columns of first = rows of second

---

## **5. Outer Product of Vectors**

Outer product → **vector × vector^T = matrix**

```python id="v5k6l7"
v1 = np.array([1,2,3])
v2 = np.array([4,5,6])

outer = np.outer(v1, v2)
print(outer)
# [[ 4  5  6]
#  [ 8 10 12]
#  [12 15 18]]
```

* Useful in **linear algebra and ML** (covariance matrices, rank-1 matrices)

---

## **6. Element-wise Multiplication (Hadamard Product)**

```python id="v6m7n8"
a = np.array([[1,2],[3,4]])
b = np.array([[5,6],[7,8]])

elementwise = a * b
print(elementwise)
# [[ 5 12]
#  [21 32]]
```

* **Different from dot product**

---

## **7. Summary Table**

| Operation                   | NumPy Function / Syntax    | Result Type |
| --------------------------- | -------------------------- | ----------- |
| Dot Product (vector)        | `np.dot(v1,v2)` or `v1@v2` | Scalar      |
| Cross Product (vector)      | `np.cross(v1,v2)`          | Vector (3D) |
| Matrix × Vector             | `A @ v` or `np.dot(A,v)`   | Vector      |
| Matrix × Matrix             | `A @ B` or `np.dot(A,B)`   | Matrix      |
| Outer Product (vectors)     | `np.outer(v1,v2)`          | Matrix      |
| Element-wise Multiplication | `A * B`                    | Matrix      |

---

💡 **Tips:**

1. Dot & Matrix product → **linear algebra / ML / DL me common**
2. Element-wise multiplication → **Hadamard product**
3. Outer product → **rank-1 matrix construction, covariance**
4. Cross product → **3D vector perpendicular calculation**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme dot product, cross product, matrix-vector, matrix-matrix, outer product, element-wise multiplication** sab ek diagram me dikh rahe ho, jisse **concept instantly clear** ho jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Determinants aur Inverse of a Matrix** detail me samjhenge. Ye **linear algebra ke fundamental concepts** hain, specially **ML, DL, aur scientific computing me**.

---

## **1. Determinant of a Matrix**

**Determinant** = square matrix ka **scalar value**, jo matrix ke properties describe karta hai:

* `det(A) = 0` → matrix **singular** hai, inverse nahi hota
* `det(A) ≠ 0` → matrix **invertible** hai

**NumPy me:** `np.linalg.det()`

```python id="d1a2b3"
import numpy as np

A = np.array([[1,2],
              [3,4]])

det = np.linalg.det(A)
print("Determinant:", det)
# Output: -2.0
```

* Formula (2x2): `det([[a,b],[c,d]]) = a*d - b*c`
* 3x3 aur higher: **recursive calculation**

---

### **Example: 3x3 Matrix**

```python id="d2c3d4"
B = np.array([[2,1,3],
              [1,0,2],
              [4,1,8]])

det_B = np.linalg.det(B)
print("Determinant of B:", det_B)
```

* Result: Scalar value

---

## **2. Inverse of a Matrix**

**Inverse** = A^-1, matrix jo original matrix ke sath multiply karne par **identity matrix** deti hai:

* Rule: Only **square matrices** with **det ≠ 0**
* NumPy function: `np.linalg.inv()`

```python id="d3e4f5"
A_inv = np.linalg.inv(A)
print("Inverse of A:\n", A_inv)
```

**Output:**

```
[[-2.   1. ]
 [ 1.5 -0.5]]
```

---

### **Check Identity Matrix**

```python id="d4f5g6"
I = np.dot(A, A_inv)
print(np.round(I,2))  # round to 2 decimals
# [[1. 0.]
#  [0. 1.]]
```

* Multiplying original matrix with its inverse → identity matrix

---

## **3. NumPy Functions for Determinant & Inverse**

| Operation       | NumPy Function     | Example                 |
| --------------- | ------------------ | ----------------------- |
| Determinant     | `np.linalg.det(A)` | `det([[1,2],[3,4]])=-2` |
| Inverse         | `np.linalg.inv(A)` | `inv([[1,2],[3,4]])`    |
| Identity Matrix | `np.eye(n)`        | `eye(3)` → 3x3 identity |
| Round values    | `np.round(arr, 2)` | Round to 2 decimals     |

---

## **4. Tips**

1. **Only square matrices** ke liye determinant aur inverse possible hai.
2. `det = 0` → **matrix singular**, inverse nahi hota.
3. **Use `np.round()`** after inverse to avoid **floating point approximation errors**.
4. Matrix inverse ML me **linear regression, PCA, solving linear equations** me bohot use hota hai.

---

Agar chaho, main **ek visual diagram bana doon jisme determinant aur inverse ka concept + check identity** dikh raha ho, jisse **quick reference aur concept clarity** mil jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Inner aur Outer Products** ko detail me samjhenge. Ye **linear algebra aur ML me fundamental concepts** hain.

---

## **1. Inner Product (Dot Product)**

**Inner product** = 2 vectors ka **sum of products of corresponding elements**.

* Scalar value return karta hai (for 1D vectors)
* NumPy function: `np.inner()` ya `np.dot()`

---

### **Example: 1D Vectors**

```python
import numpy as np

v1 = np.array([1,2,3])
v2 = np.array([4,5,6])

inner = np.inner(v1, v2)
print("Inner Product:", inner)
# Output: 1*4 + 2*5 + 3*6 = 32
```

* Same as dot product

---

### **Example: 2D Arrays**

```python
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

inner2d = np.inner(A, B)
print("Inner Product 2D:\n", inner2d)
```

**Output explanation:**

* Each **row of A** dot **with each row of B**
* Result: 2x2 matrix

---

## **2. Outer Product**

**Outer product** = **vector × vector^T** → **matrix** return karta hai

* NumPy function: `np.outer()`

---

### **Example: 1D Vectors**

```python
v1 = np.array([1,2,3])
v2 = np.array([4,5,6])

outer = np.outer(v1, v2)
print("Outer Product:\n", outer)
```

**Output:**

```
[[ 4  5  6]
 [ 8 10 12]
 [12 15 18]]
```

* Result = **rows = len(v1), columns = len(v2)**
* Useful in **linear algebra, rank-1 matrices, covariance matrices**

---

## **3. Key Differences**

| Feature            | Inner Product (`np.inner`) | Outer Product (`np.outer`)                |
| ------------------ | -------------------------- | ----------------------------------------- |
| Output             | Scalar (1D) / Matrix (2D)  | Matrix                                    |
| Formula            | sum(a[i]*b[i])             | a[i]*b[j] for all i,j                     |
| Shape (1D vectors) | ()                         | (len(a), len(b))                          |
| Use Cases          | Projection, dot product    | Rank-1 matrix, covariance, linear algebra |

---

## **4. Quick Example with 1D and 2D**

```python
# 1D vectors
v1 = np.array([1,2])
v2 = np.array([3,4])

print("Inner:", np.inner(v1, v2))  # 1*3 + 2*4 = 11
print("Outer:\n", np.outer(v1, v2))
# [[3 4]
#  [6 8]]
```

```python
# 2D arrays
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

print("Inner 2D:\n", np.inner(A,B))
# [[17 23]
#  [39 53]]

print("Outer 2D:\n", np.outer(A,B))
# 4x4 matrix
```

---

💡 **Tips:**

1. **Inner product** → vector similarity, projection, dot product
2. **Outer product** → matrix construction, covariance, rank-1 matrix
3. **np.dot()**, `@` → alternate for inner product (especially in ML & DL)

---

Agar chaho, main **ek visual cheat sheet bana doon jisme inner aur outer product ka **1D aur 2D examples + result matrix** diagram me dikh rahe ho**, jisse concept **instant samajh aaye**.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy ke `dot()` aur `vdot()` functions** ko detail me samjhenge. Ye **vector aur matrix operations ke liye important** hain, lekin in dono me subtle differences hote hain.

---

## **1. `np.dot()` Function**

**`np.dot()`** ka use **dot product / matrix multiplication** ke liye hota hai:

* 1D arrays → **dot product (scalar)**
* 2D arrays → **matrix multiplication**
* Higher dimensions → **sum product over last axis of a and second-last axis of b**

---

### **Example 1: 1D Vectors**

```python id="dot1"
import numpy as np

a = np.array([1,2,3])
b = np.array([4,5,6])

result = np.dot(a, b)
print(result)
# Output: 1*4 + 2*5 + 3*6 = 32
```

---

### **Example 2: 2D Matrices**

```python id="dot2"
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

result = np.dot(A, B)
print(result)
# Output:
# [[19 22]
#  [43 50]]
```

* **Columns of A** multiply **rows of B** → standard matrix multiplication

---

### **Example 3: Broadcasting / Higher Dimensions**

```python id="dot3"
a = np.array([[1,2],[3,4]])
b = np.array([10,20])
print(np.dot(a,b))
# [[1*10+2*20], [3*10+4*20]] → [50 110]
```

---

## **2. `np.vdot()` Function**

**`np.vdot()`** bhi **dot product** calculate karta hai, lekin **special rule** hai:

* Both inputs **flattened to 1D** before computing dot product
* Complex numbers → **complex conjugate** of the first vector is taken

---

### **Example 1: 1D Vectors**

```python id="vdot1"
a = np.array([1,2,3])
b = np.array([4,5,6])

result = np.vdot(a, b)
print(result)
# Output: 32 (same as np.dot for 1D real numbers)
```

---

### **Example 2: 2D Arrays Flattened**

```python id="vdot2"
A = np.array([[1,2],[3,4]])
B = np.array([[5,6],[7,8]])

result = np.vdot(A,B)
print(result)
# Output: 1*5 + 2*6 + 3*7 + 4*8 = 70
```

* Note: `np.dot(A,B)` → matrix multiplication (2x2)
* `np.vdot(A,B)` → flatten → scalar sum

---

### **Example 3: Complex Numbers**

```python id="vdot3"
a = np.array([1+2j, 3+4j])
b = np.array([5+6j, 7+8j])

print(np.dot(a,b))   # standard dot, no conjugate
print(np.vdot(a,b))  # conjugate(a) * b, scalar
```

* `vdot` **complex conjugate** use karta hai → result different ho sakta hai

---

## **3. Key Differences: `dot()` vs `vdot()`**

| Feature         | `np.dot()`                          | `np.vdot()`                                          |
| --------------- | ----------------------------------- | ---------------------------------------------------- |
| Input shape     | Preserves shape (1D or 2D)          | Flattens inputs to 1D                                |
| Output          | Scalar (1D) / Matrix (2D)           | Always scalar                                        |
| Complex numbers | No conjugate                        | Conjugates first input                               |
| Use case        | Matrix multiplication / dot product | Flattened dot product, conjugate for complex numbers |

---

💡 **Tips:**

1. **1D real arrays:** `dot()` = `vdot()`
2. **2D arrays:** `dot()` → matrix multiplication, `vdot()` → scalar sum of flattened
3. **Complex numbers:** `vdot()` automatically **conjugates** first input

---

Agar chaho, main **ek visual diagram bana doon jisme `dot()` vs `vdot()` ka 1D, 2D aur complex number example** dikh raha ho, jisse concept **instant clear ho jaye**.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Eigenvalues aur Eigenvectors** ko detail me samjhenge. Ye **linear algebra ke core concepts** hain aur **ML, PCA, physics, engineering** me extensively use hote hain.

---

## **1. Eigenvalues & Eigenvectors Kya Hain?**

For a square matrix **A**:

[
A \mathbf{v} = \lambda \mathbf{v}
]

* **v** → Eigenvector → direction jo matrix transform hone par **same direction me** rehta hai
* **λ** → Eigenvalue → scaling factor jo eigenvector ke sath multiply hota hai

**Intuition:**

* Eigenvectors → matrix ke “special directions”
* Eigenvalues → matrix ke “stretch/compress factor” along eigenvectors

---

## **2. NumPy Functions**

NumPy me **`np.linalg.eig()`** ka use hota hai:

```python id="eig1"
import numpy as np

A = np.array([[2, 1],
              [1, 2]])

eigvals, eigvecs = np.linalg.eig(A)
print("Eigenvalues:", eigvals)
print("Eigenvectors:\n", eigvecs)
```

**Output Example:**

```
Eigenvalues: [3. 1.]
Eigenvectors:
 [[ 0.70710678 -0.70710678]
  [ 0.70710678  0.70710678]]
```

* `eigvals` → eigenvalues
* `eigvecs` → columns of eigenvectors

---

## **3. Verification**

Eigenvector & eigenvalue verify karne ke liye:

```python id="eig2"
for i in range(len(eigvals)):
    Av = A @ eigvecs[:,i]
    lv = eigvals[i] * eigvecs[:,i]
    print(np.allclose(Av, lv))  # True if correct
```

* `np.allclose()` → floating point comparison

---

## **4. 3x3 Matrix Example**

```python id="eig3"
B = np.array([[1,2,3],
              [0,1,4],
              [5,6,0]])

eigvals, eigvecs = np.linalg.eig(B)
print("Eigenvalues:", eigvals)
print("Eigenvectors:\n", eigvecs)
```

* Eigenvalues → scalar (possibly complex)
* Eigenvectors → each column corresponds to eigenvalue

---

## **5. Key Notes**

1. **Eigenvalues can be complex** → especially for non-symmetric matrices
2. **Eigenvectors can be scaled** → any multiple is valid
3. **Symmetric matrices** → eigenvalues real, eigenvectors orthogonal

---

## **6. Practical Use Cases**

* **PCA (Principal Component Analysis)** → dimensionality reduction
* **Physics/Engineering** → vibration modes, stability analysis
* **ML / Data Science** → covariance matrix decomposition

---

## **7. Quick Summary Table**

| Concept                      | NumPy Function                                  | Notes                                      |
| ---------------------------- | ----------------------------------------------- | ------------------------------------------ |
| Eigenvalues & Eigenvectors   | `np.linalg.eig(A)`                              | A must be square                           |
| Symmetric matrix eigenvalues | `np.linalg.eigh(A)`                             | Optimized for symmetric/hermitian matrices |
| Verification                 | `A @ v = λ * v`                                 | Check with `np.allclose()`                 |
| Shape                        | `eigvals.shape = (n,)`, `eigvecs.shape = (n,n)` | Columns = eigenvectors                     |

---

💡 **Tips:**

1. **Always use square matrices**
2. **Symmetric matrices** → use `np.linalg.eigh()` → faster & stable
3. **Eigenvectors are column-wise** in the output

---

Agar chaho, main **ek visual diagram bana doon jisme 2x2 matrix ke eigenvectors & eigenvalues, unka direction aur scaling factor** dikh raha ho, jisse **intuition instantly samajh aaye**.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Random Numbers generate karna** detail me samjhenge. Ye **simulation, testing, ML initialization** ke liye bohot important hai.

---

## **1. NumPy Random Module**

NumPy me **`numpy.random`** module use hota hai **random numbers generate karne ke liye**:

```python id="rand1"
import numpy as np
```

---

## **2. Random Numbers Between 0 and 1**

```python id="rand2"
arr = np.random.rand(5)  # 1D array of 5 elements
print(arr)
# Example Output: [0.5488135  0.71518937 0.60276338 0.54488318 0.4236548 ]
```

* **Uniform distribution**: 0 se 1 ke beech

```python id="rand3"
arr2 = np.random.rand(2,3)  # 2x3 matrix
print(arr2)
```

---

## **3. Standard Normal Distribution**

```python id="rand4"
arr = np.random.randn(5)  # mean=0, std=1
print(arr)
# Example Output: [-0.23415337  0.23413696  0.00972872 -0.23514532 0.43387597]
```

* **Normal/Gaussian distribution**
* Useful in **ML, weight initialization**

---

## **4. Random Integers**

```python id="rand5"
arr = np.random.randint(10, 50, size=5)  # 5 integers from 10 to 49
print(arr)
# Example Output: [12 25 43 33 17]
```

* Syntax: `randint(low, high, size)`
* High excluded

---

## **5. Random Choice from Array**

```python id="rand6"
arr = np.array([10,20,30,40,50])
rand_sample = np.random.choice(arr, size=3)
print(rand_sample)
# Example Output: [20 40 10]
```

* Randomly pick elements from array
* Optional: `replace=False` → no repetition

---

## **6. Shuffle Array**

```python id="rand7"
arr = np.array([1,2,3,4,5])
np.random.shuffle(arr)
print(arr)
# Example Output: [3 5 1 2 4]
```

* **In-place shuffle**

---

## **7. Seed for Reproducibility**

```python id="rand8"
np.random.seed(42)  # same random numbers every time
print(np.random.rand(3))
# Output: [0.37454012 0.95071431 0.73199394]
```

* Important for **experiments, ML model reproducibility**

---

## **8. Summary Table**

| Function                             | Description                     | Example                |
| ------------------------------------ | ------------------------------- | ---------------------- |
| `np.random.rand(d0,d1,...)`          | Uniform [0,1]                   | `rand(3)`              |
| `np.random.randn(d0,d1,...)`         | Standard Normal (mean=0, std=1) | `randn(3)`             |
| `np.random.randint(low, high, size)` | Random integers                 | `randint(10,50,5)`     |
| `np.random.choice(arr, size)`        | Random selection from array     | `choice([10,20,30],2)` |
| `np.random.shuffle(arr)`             | Shuffle array in-place          | `shuffle([1,2,3])`     |
| `np.random.seed(n)`                  | Set seed for reproducibility    | `seed(42)`             |

---

💡 **Tips:**

1. **`seed()`** → experiments ko repeatable banata hai
2. **rand vs randn** → uniform vs normal distribution
3. **choice & shuffle** → data sampling aur permutation ke liye useful

---

Agar chaho, main **ek visual cheat sheet bana doon jisme rand, randn, randint, choice, shuffle, seed ka example output** diagram me dikh raha ho, jisse **quick reference** ban jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Normal Distribution** ko detail me samjhenge. Ye **statistics, probability, ML, data science** me bohot common hai.

---

## **1. Normal Distribution Kya Hai?**

**Normal Distribution** = bell-shaped curve, jisme:

* **Mean (μ)** → center
* **Standard Deviation (σ)** → spread
* 68-95-99.7 rule → data ~68% within 1σ, 95% within 2σ, 99.7% within 3σ

**Probability Density Function (PDF):**

[
f(x) = \frac{1}{\sigma \sqrt{2\pi}} e^{-\frac{(x-\mu)^2}{2\sigma^2}}
]

---

## **2. Generate Normal Random Numbers in NumPy**

### **Using `np.random.randn()` (Standard Normal)**

```python id="norm1"
import numpy as np

# Standard normal: mean=0, std=1
arr = np.random.randn(5)
print(arr)
# Example Output: [ 0.49671415 -0.1382643  0.64768854 1.52302986 -0.23415337 ]
```

* Always **mean=0, std=1**
* Shape can be 1D, 2D, etc.

---

### **Using `np.random.normal()` (Custom μ, σ)**

```python id="norm2"
# mean=10, std=2, 5 samples
arr = np.random.normal(loc=10, scale=2, size=5)
print(arr)
# Example Output: [11.329, 9.837, 10.241, 12.153, 8.932]
```

* `loc` → mean μ
* `scale` → standard deviation σ
* `size` → number of samples

---

### **2D Normal Distribution**

```python id="norm3"
arr2d = np.random.normal(loc=0, scale=1, size=(3,4))
print(arr2d)
```

* Result → 3x4 matrix, all elements random from normal distribution

---

## **3. Visualizing Normal Distribution**

```python id="norm4"
import matplotlib.pyplot as plt

data = np.random.normal(loc=0, scale=1, size=1000)
plt.hist(data, bins=30, density=True, color='skyblue')
plt.title("Normal Distribution")
plt.show()
```

* Histogram → bell-shaped curve

---

## **4. Properties / Tips**

1. **`randn()`** → always **standard normal**
2. **`normal(loc, scale, size)`** → custom mean & std
3. **`size`** → array shape
4. **Use in ML:** weight initialization, noise addition, synthetic data generation

---

## **5. Quick Comparison Table**

| Function                             | Description                       | Example          |
| ------------------------------------ | --------------------------------- | ---------------- |
| `np.random.randn(d0,d1)`             | Standard normal (mean=0, std=1)   | `randn(5)`       |
| `np.random.normal(loc, scale, size)` | Normal with custom mean μ & std σ | `normal(10,2,5)` |

---

💡 **Tips:**

* Always **use seed** (`np.random.seed(42)`) for reproducibility
* Visualize histogram → check **bell curve shape**
* ML me often **weights, noise, synthetic datasets** me use hota hai

---

Agar chaho, main **ek visual cheat sheet bana doon jisme randn vs normal, 1D & 2D examples aur histogram** sab ek diagram me dikh raha ho, jisse **instant reference** ban jaye.

Chahte ho main wo bana doon?



Perfect! Ab hum **NumPy me Binomial Distribution** ko detail me samjhenge. Ye **probability aur statistics ke liye core concept** hai, aur ML me bhi bohot useful hai.

---

## **1. Binomial Distribution Kya Hai?**

**Binomial Distribution** → probability distribution for **number of successes** in a **fixed number of independent trials**:

* **n** → number of trials
* **p** → probability of success in each trial
* **k** → number of successes

**Probability Mass Function (PMF):**

[
P(X=k) = \binom{n}{k} p^k (1-p)^{n-k}
]

**Intuition:**

* Example: coin toss 10 times, probability of getting exactly 6 heads

---

## **2. NumPy Function: `np.random.binomial()`**

```python id="bin1"
import numpy as np

# Parameters
n = 10      # trials
p = 0.5     # probability of success
size = 5    # number of experiments

arr = np.random.binomial(n, p, size)
print(arr)
# Example Output: [5 6 4 7 3]
```

* Each element → **number of successes in n trials**

---

### **2D Binomial Array**

```python id="bin2"
arr2d = np.random.binomial(n=10, p=0.5, size=(3,4))
print(arr2d)
# Example Output:
# [[4 6 5 7]
#  [5 3 4 6]
#  [6 4 3 5]]
```

* 3x4 matrix → each element independent trial outcome

---

## **3. Visualization**

```python id="bin3"
import matplotlib.pyplot as plt

data = np.random.binomial(n=10, p=0.5, size=1000)
plt.hist(data, bins=11, density=True, color='lightgreen', edgecolor='black')
plt.title("Binomial Distribution (n=10, p=0.5)")
plt.xlabel("Number of Successes")
plt.ylabel("Probability")
plt.show()
```

* Histogram → shows distribution of successes

---

## **4. Key Properties**

1. **Mean (Expected value):** μ = n * p
2. **Variance:** σ² = n * p * (1-p)
3. **Use case:** Coin toss, defect items, success/failure events, ML simulations

---

## **5. Quick Reference Table**

| Function                         | Description                     | Example                |
| -------------------------------- | ------------------------------- | ---------------------- |
| `np.random.binomial(n, p, size)` | Number of successes in n trials | `binomial(10, 0.5, 5)` |

---

💡 **Tips:**

* Always **size parameter** → how many samples you want
* For **large n & p ≈ 0.5**, binomial ~ **normal distribution** (Central Limit Theorem)
* Useful in **probability simulations, ML experiments, A/B testing**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme binomial distribution ka 1D aur 2D example + histogram** dikh raha ho, jisse concept **instant samajh aaye**.

Chahte ho main wo bana doon?



Perfect! Ab hum **NumPy me Poisson Distribution** ko detail me samjhenge. Ye **probability, statistics, aur ML** me kaafi important hai, specially **count-based events** ke liye.

---

## **1. Poisson Distribution Kya Hai?**

**Poisson Distribution** → probability distribution for **number of events in a fixed interval of time or space**, given **average rate λ (lambda)**:

* λ → average number of events per interval
* k → actual number of events (0,1,2,…)

**Probability Mass Function (PMF):**

[
P(X=k) = \frac{e^{-\lambda} \lambda^k}{k!}
]

**Intuition:**

* Example: 1 hour me average 5 calls aate hain, probability exactly 3 calls aane ki

---

## **2. NumPy Function: `np.random.poisson()`**

```python id="pois1"
import numpy as np

lam = 5      # average number of events
size = 10    # number of samples

arr = np.random.poisson(lam, size)
print(arr)
# Example Output: [4 5 3 6 5 7 4 2 8 5]
```

* Each element → **number of events in interval**

---

### **2D Poisson Array**

```python id="pois2"
arr2d = np.random.poisson(lam=5, size=(3,4))
print(arr2d)
# Example Output:
# [[4 5 3 6]
#  [5 7 4 2]
#  [8 5 6 3]]
```

* 3x4 matrix → independent Poisson samples

---

## **3. Visualization**

```python id="pois3"
import matplotlib.pyplot as plt

data = np.random.poisson(lam=5, size=1000)
plt.hist(data, bins=15, density=True, color='lightcoral', edgecolor='black')
plt.title("Poisson Distribution (λ=5)")
plt.xlabel("Number of Events")
plt.ylabel("Probability")
plt.show()
```

* Histogram → discrete distribution, skewed slightly for smaller λ

---

## **4. Key Properties**

1. **Mean:** μ = λ
2. **Variance:** σ² = λ
3. **Use case:**

   * Number of phone calls per hour
   * Number of arrivals per day
   * Events per unit in ML simulations

---

## **5. Quick Reference Table**

| Function                       | Description                              | Example         |
| ------------------------------ | ---------------------------------------- | --------------- |
| `np.random.poisson(lam, size)` | Random numbers from Poisson distribution | `poisson(5,10)` |

---

💡 **Tips:**

1. λ small → distribution skewed, λ large → approaches normal distribution
2. Always set **size** for number of samples
3. Useful in **queueing theory, traffic modeling, ML event simulations**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme poisson distribution ke 1D aur 2D examples + histogram** dikh rahe ho, jisse concept **instant samajh aaye**.

Chahte ho main wo bana doon?



Perfect! Ab hum **NumPy me Uniform Distribution** ko detail me samjhenge. Ye **statistics, simulation, and ML** me bohot commonly use hota hai.

---

## **1. Uniform Distribution Kya Hai?**

**Uniform Distribution** → probability distribution jisme **sab values equally likely** hoti hain **ek interval [low, high] me**.

* Continuous Uniform → real numbers in interval [a,b]
* Discrete Uniform → integers with equal probability

**Probability Density Function (PDF):**

[
f(x) = \frac{1}{b-a}, \quad a \le x \le b
]

**Intuition:**

* Example: Random number generator → 0 se 1 ke beech har number equally likely

---

## **2. NumPy Functions for Uniform Distribution**

### **2.1 Continuous Uniform: `np.random.rand()`**

```python id="uni1"
import numpy as np

# 1D array of 5 elements in [0,1)
arr = np.random.rand(5)
print(arr)
# Example Output: [0.37454012 0.95071431 0.73199394 0.59865848 0.15601864]
```

* Uniform numbers **0 ≤ x < 1**
* 2D array:

```python id="uni2"
arr2d = np.random.rand(3,4)  # 3x4 matrix
print(arr2d)
```

---

### **2.2 Continuous Uniform with Custom Interval: `np.random.uniform(low, high, size)`**

```python id="uni3"
arr = np.random.uniform(low=10, high=20, size=5)
print(arr)
# Example Output: [13.548, 19.234, 11.987, 14.321, 17.543]
```

* `low` → minimum value
* `high` → maximum value
* `size` → number of samples

---

### **2.3 Discrete Uniform: `np.random.randint(low, high, size)`**

```python id="uni4"
arr = np.random.randint(1, 7, size=5)  # dice roll
print(arr)
# Example Output: [3 6 1 4 2]
```

* Only integers in `[low, high-1]`

---

## **3. Visualization**

```python id="uni5"
import matplotlib.pyplot as plt

data = np.random.uniform(low=0, high=1, size=1000)
plt.hist(data, bins=20, density=True, color='lightblue', edgecolor='black')
plt.title("Uniform Distribution [0,1]")
plt.xlabel("Value")
plt.ylabel("Probability")
plt.show()
```

* Histogram → flat, all values equally likely

---

## **4. Key Properties**

1. **Mean:** μ = (a+b)/2
2. **Variance:** σ² = (b-a)² / 12
3. **Use Cases:**

   * Random sampling
   * ML weight initialization
   * Simulations / testing

---

## **5. Quick Reference Table**

| Function                             | Description                       | Example            |
| ------------------------------------ | --------------------------------- | ------------------ |
| `np.random.rand(d0,d1,...)`          | Standard continuous uniform [0,1) | `rand(5)`          |
| `np.random.uniform(low, high, size)` | Continuous uniform [low, high)    | `uniform(10,20,5)` |
| `np.random.randint(low, high, size)` | Discrete uniform integers         | `randint(1,7,5)`   |

---

💡 **Tips:**

* Use `seed()` for reproducibility: `np.random.seed(42)`
* `rand()` → simple uniform [0,1)
* `uniform(low, high)` → custom interval
* Discrete uniform → random integers

---

Agar chaho, main **ek visual cheat sheet bana doon jisme uniform distribution ke rand, uniform, randint examples + histogram** sab ek diagram me dikh raha ho, jisse **instant reference aur clarity** mil jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Exponential Distribution** ko detail me samjhenge. Ye **statistics, queuing theory, ML, reliability analysis** me bohot common hai.

---

## **1. Exponential Distribution Kya Hai?**

**Exponential Distribution** → probability distribution jo **time between events in a Poisson process** describe karta hai.

* λ → rate parameter (events per unit time)
* x → time until next event

**Probability Density Function (PDF):**

[
f(x) = \lambda e^{-\lambda x}, \quad x \ge 0
]

**Intuition:**

* Example: Phone call center me next call kab aayega → exponential distribution model

---

## **2. NumPy Function: `np.random.exponential()`**

```python id="exp1"
import numpy as np

scale = 2.0   # scale = 1/λ
size = 5

arr = np.random.exponential(scale=scale, size=size)
print(arr)
# Example Output: [1.234 0.567 3.456 2.789 0.987]
```

* **scale** = 1/λ
* **size** → number of samples

---

### **2D Exponential Array**

```python id="exp2"
arr2d = np.random.exponential(scale=1.5, size=(3,4))
print(arr2d)
```

* Result → 3x4 matrix, independent exponential samples

---

## **3. Visualization**

```python id="exp3"
import matplotlib.pyplot as plt

data = np.random.exponential(scale=1.0, size=1000)
plt.hist(data, bins=30, density=True, color='lightpink', edgecolor='black')
plt.title("Exponential Distribution (λ=1)")
plt.xlabel("x")
plt.ylabel("Probability")
plt.show()
```

* Histogram → rapidly decreasing curve
* Most values near 0, tail decreases exponentially

---

## **4. Key Properties**

1. **Mean:** μ = scale = 1/λ
2. **Variance:** σ² = (scale)² = 1/λ²
3. **Use Cases:**

   * Time between Poisson events (calls, arrivals)
   * Lifetime of devices / reliability
   * ML → sampling, noise, synthetic data

---

## **5. Quick Reference Table**

| Function                             | Description                                  | Example               |
| ------------------------------------ | -------------------------------------------- | --------------------- |
| `np.random.exponential(scale, size)` | Random numbers from exponential distribution | `exponential(2.0, 5)` |

---

💡 **Tips:**

* **scale = 1/λ** → remember to convert if you have λ instead of scale
* Histogram → skewed right, always ≥ 0
* Useful in **queue simulations, reliability testing, ML synthetic data**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme exponential distribution ke 1D aur 2D examples + histogram** sab ek diagram me dikh raha ho, jisse **instant reference aur clarity** mil jaye.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Chi-Square Distribution** ko detail me samjhenge. Ye **statistics, hypothesis testing, ML, and data science** me bohot common hai.

---

## **1. Chi-Square Distribution Kya Hai?**

**Chi-Square Distribution** → probability distribution jo **sum of squares of k independent standard normal variables** ka distribution describe karta hai.

* k → degrees of freedom (df)
* Always **non-negative**
* Skewed distribution, right tail longer for small df

**Intuition:**

* Example: Observed vs expected frequencies in **Chi-Square test**
* ML: Feature independence testing

---

## **2. NumPy Function: `np.random.chisquare()`**

```python id="chi1"
import numpy as np

df = 4       # degrees of freedom
size = 5

arr = np.random.chisquare(df, size)
print(arr)
# Example Output: [3.12 5.45 1.87 4.33 2.56]
```

* Each element → chi-square random variable
* **df** = number of independent standard normal variables squared

---

### **2D Chi-Square Array**

```python id="chi2"
arr2d = np.random.chisquare(df=3, size=(3,4))
print(arr2d)
```

* Result → 3x4 matrix, independent chi-square samples

---

## **3. Visualization**

```python id="chi3"
import matplotlib.pyplot as plt

data = np.random.chisquare(df=4, size=1000)
plt.hist(data, bins=30, density=True, color='lightyellow', edgecolor='black')
plt.title("Chi-Square Distribution (df=4)")
plt.xlabel("Value")
plt.ylabel("Probability")
plt.show()
```

* Histogram → skewed right, non-negative values

---

## **4. Key Properties**

1. **Mean:** μ = df
2. **Variance:** σ² = 2 * df
3. **Skewness:** right-skewed for small df, approx normal for large df
4. **Use Cases:**

   * Hypothesis testing (goodness-of-fit, independence)
   * ML → feature selection, covariance tests
   * Simulating sums of squared normals

---

## **5. Quick Reference Table**

| Function                        | Description                             | Example          |
| ------------------------------- | --------------------------------------- | ---------------- |
| `np.random.chisquare(df, size)` | Chi-square random numbers with given df | `chisquare(4,5)` |

---

💡 **Tips:**

* **Always df > 0**
* For **large df**, chi-square ~ normal distribution
* Histogram → **non-negative, right-skewed**
* Use in **statistical tests, ML feature evaluation**

---

Agar chaho, main **ek visual cheat sheet bana doon jisme chi-square distribution ke 1D aur 2D examples + histogram** sab ek diagram me dikh raha ho, jisse concept **instant samajh aaye**.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy me Statistical Functions** detail me samjhenge, jisme **mean, median, variance aur standard deviation** included hain. Ye **data analysis, ML, aur statistics** ke core concepts hain.

---

## **1. Mean (Average)**

**Mean** = sum of all elements ÷ number of elements

```python id="stat1"
import numpy as np

arr = np.array([1,2,3,4,5])

mean_val = np.mean(arr)
print("Mean:", mean_val)
# Output: 3.0
```

* **Axis parameter:** axis=0 → column-wise, axis=1 → row-wise (2D arrays)

```python id="stat2"
arr2d = np.array([[1,2,3],[4,5,6]])
print("Mean along axis 0:", np.mean(arr2d, axis=0))  # [2.5 3.5 4.5]
print("Mean along axis 1:", np.mean(arr2d, axis=1))  # [2.0 5.0]
```

---

## **2. Median**

**Median** = middle value (sorted array)

```python id="stat3"
median_val = np.median(arr)
print("Median:", median_val)
# Output: 3
```

* Even number of elements → average of 2 middle elements

```python id="stat4"
arr_even = np.array([1,2,3,4])
print("Median:", np.median(arr_even))  # 2.5
```

---

## **3. Variance**

**Variance (σ²)** = average of squared differences from mean

[
\sigma^2 = \frac{1}{N} \sum (x_i - \mu)^2
]

```python id="stat5"
var_val = np.var(arr)
print("Variance:", var_val)
# Output: 2.0
```

* **Axis parameter** → same as mean

```python id="stat6"
print("Variance along axis 0:", np.var(arr2d, axis=0))  # [2.25 2.25 2.25]
print("Variance along axis 1:", np.var(arr2d, axis=1))  # [0.6667 0.6667]
```

---

## **4. Standard Deviation**

**Standard Deviation (σ)** = sqrt of variance

```python id="stat7"
std_val = np.std(arr)
print("Standard Deviation:", std_val)
# Output: 1.4142135623730951
```

* **Axis parameter** → same as mean & variance

```python id="stat8"
print("Std along axis 0:", np.std(arr2d, axis=0))  # [1.5 1.5 1.5]
print("Std along axis 1:", np.std(arr2d, axis=1))  # [0.8165 0.8165]
```

---

## **5. Quick Reference Table**

| Function         | Description                                 | Example |
| ---------------- | ------------------------------------------- | ------- |
| `np.mean(arr)`   | Average of elements                         | 3.0     |
| `np.median(arr)` | Middle value                                | 3       |
| `np.var(arr)`    | Variance                                    | 2.0     |
| `np.std(arr)`    | Standard deviation                          | 1.414   |
| Axis parameter   | `axis=0` → column-wise, `axis=1` → row-wise | N/A     |

---

## **6. Tips**

1. **Axis parameter** → 2D arrays me useful
2. **Variance & std** → data spread measure
3. **Median** → robust to outliers
4. Use **`np.round()`** for readable outputs

---

Agar chaho, main **ek visual cheat sheet bana doon jisme mean, median, variance, standard deviation ke formulas + 1D/2D example** diagram me dikh rahe ho, jisse **instant reference aur clarity** mil jaye.

Chahte ho main wo bana doon?



Perfect! Ab hum **NumPy me Vectorized Operations** aur unka **performance optimization** me importance ko detail me samjhenge. Ye concept **Python me high-performance numerical computing aur ML** ke liye bohot important hai.

---

## **1. Vectorized Operations Kya Hain?**

**Vectorization** → **element-wise operations without explicit loops** (for loops)

* NumPy arrays ke operations **C-level optimized** hote hain → fast
* Python loops → slow, NumPy vectorized operations → fast

---

### **Example 1: Using For Loop (Slower)**

```python id="vec1"
import numpy as np
import time

arr = np.arange(1_000_000)
start = time.time()

squared = np.zeros_like(arr)
for i in range(len(arr)):
    squared[i] = arr[i]**2

end = time.time()
print("Time with loop:", end - start)
```

---

### **Example 2: Using Vectorized NumPy Operation (Faster)**

```python id="vec2"
start = time.time()

squared_vec = arr ** 2  # vectorized
end = time.time()
print("Time with vectorized operation:", end - start)
```

* **Result:** Vectorized version bohot fast hota hai
* Python loop = seconds, Vectorized = milliseconds

---

## **2. Common Vectorized Operations**

| Operation                   | NumPy Example             | Notes                       |
| --------------------------- | ------------------------- | --------------------------- |
| Element-wise addition       | `a + b`                   | Arrays same shape           |
| Element-wise multiplication | `a * b`                   | Hadamard product            |
| Scalar operations           | `a + 10`, `a * 5`         | Broadcast applied           |
| Power / sqrt / log / exp    | `a**2`, `np.sqrt(a)`      | Universal functions (ufunc) |
| Sum / mean / min / max      | `np.sum(a)`, `np.mean(a)` | Aggregation functions       |

---

### **Example 3: Vectorized Math Operations**

```python id="vec3"
a = np.array([1,2,3,4,5])
b = np.array([10,20,30,40,50])

c = a + b          # element-wise addition
d = a * b          # element-wise multiplication
e = a**2           # element-wise power
f = np.sqrt(b)     # square root
print(c, d, e, f)
```

---

## **3. Broadcasting for Vectorization**

**Broadcasting** → smaller array automatically **expand ho jata hai** larger array ke shape ke saath operations ke liye

```python id="vec4"
a = np.array([1,2,3])
b = 10
c = a + b  # 10 is broadcasted
print(c)   # [11 12 13]
```

* 2D arrays me bhi possible

```python id="vec5"
A = np.array([[1,2,3],[4,5,6]])
B = np.array([10,20,30])
C = A + B
print(C)
# [[11 22 33]
#  [14 25 36]]
```

---

## **4. Why Vectorization Improves Performance**

1. **Loops avoided** → Python interpreter overhead eliminated
2. **C-level optimization** → NumPy internally fast
3. **Memory efficiency** → no temporary lists created
4. **Readable code** → less lines, less errors

---

## **5. Timing Comparison Example**

```python id="vec6"
import numpy as np
import time

N = 10_000_000
a = np.arange(N)

# Loop
start = time.time()
result = np.zeros(N)
for i in range(N):
    result[i] = a[i] ** 2
end = time.time()
print("Loop time:", end-start)

# Vectorized
start = time.time()
result_vec = a ** 2
end = time.time()
print("Vectorized time:", end-start)
```

* **Vectorized → 10–100x faster**

---

## **6. Tips for Using Vectorized Operations**

1. **Always prefer NumPy array operations over Python loops**
2. **Use broadcasting** instead of manually repeating arrays
3. **Use NumPy ufuncs** → optimized element-wise math functions
4. **Avoid appending in loops** → use vectorized array creation

---

💡 **Conclusion:**
Vectorized operations are **core to high-performance numerical computing**. ML, DL, and scientific computing me **vectorized code** likhna almost mandatory hai for **speed & readability**.

---

Agar chaho, main **ek visual cheat sheet bana doon jisme vectorization vs loop ka time comparison, broadcasting, element-wise operations** sab ek diagram me dikh rahe ho, jisse **instant clarity** mile.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy aur SciPy me Sparse Matrices** ko detail me samjhenge. Ye **large-scale numerical computing, ML, graph algorithms** me bohot important hai.

---

## **1. Sparse Matrix Kya Hai?**

**Sparse Matrix** → matrix jisme **zyadatar elements zero hote hain**.

* **Dense Matrix** → mostly non-zero
* **Sparse Matrix** → memory & computation efficiently store hoti hai

**Intuition:**

* Example: Social network adjacency matrix, recommender systems, graph edges
* Agar 1 million × 1 million matrix hai aur only 0.1% non-zero → sparse matrix ka use memory save karta hai

---

## **2. SciPy Sparse Matrix Module**

NumPy **direct sparse matrix support nahi karta**, lekin **SciPy** me multiple formats hote hain:

```python id="sparse1"
from scipy import sparse
import numpy as np
```

---

### **2.1 Creating Sparse Matrix from Dense Matrix**

```python id="sparse2"
dense = np.array([[0,0,1],
                  [1,0,0],
                  [0,0,0]])

sparse_matrix = sparse.csr_matrix(dense)  # CSR format
print(sparse_matrix)
```

**Output:**

```
  (0, 2)    1
  (1, 0)    1
```

* Only non-zero elements stored
* CSR = Compressed Sparse Row → efficient row slicing

---

### **2.2 Sparse Matrix Formats**

| Format       | Description              | Best Use                                     |
| ------------ | ------------------------ | -------------------------------------------- |
| `csr_matrix` | Compressed Sparse Row    | Row operations, matrix-vector multiplication |
| `csc_matrix` | Compressed Sparse Column | Column operations, fast slicing              |
| `coo_matrix` | Coordinate list          | Constructing sparse matrix from scratch      |
| `dok_matrix` | Dictionary of keys       | Incremental construction                     |

---

### **2.3 COO Format Example**

```python id="sparse3"
coo = sparse.coo_matrix(dense)
print("Data:", coo.data)
print("Row indices:", coo.row)
print("Col indices:", coo.col)
```

* Stores **(row, col, value)** for non-zero entries

---

## **3. Sparse Matrix Operations**

* Arithmetic operations supported (addition, multiplication)
* Matrix-vector multiplication efficient

```python id="sparse4"
v = np.array([1,2,3])
result = sparse_matrix.dot(v)
print(result)  # Output: [3 1 0]
```

* Only non-zero multiplications → fast

---

## **4. Memory Efficiency Example**

```python id="sparse5"
dense = np.zeros((1000,1000))
dense[10,20] = 5
dense[500,600] = 3

sparse_mtx = sparse.csr_matrix(dense)
print("Dense size:", dense.nbytes)
print("Sparse size:", sparse_mtx.data.nbytes)
```

* Sparse → stores only non-zero → **huge memory saving**

---

## **5. Use Cases**

1. **Graph adjacency matrices** → social networks, roads
2. **Recommender systems** → user-item matrices
3. **ML algorithms** → NLP bag-of-words, TF-IDF vectors
4. **Scientific computing** → FEM (finite element method)

---

## **6. Tips**

* Always **use sparse matrices** for large matrices with mostly zeros
* **CSR** → efficient row-wise computation
* **COO / DOK** → incremental construction
* Convert to dense only for **small matrices** for visualization

---

💡 **Conclusion:**
Sparse matrices → **memory-efficient storage + fast computation** for large, mostly-zero datasets. SciPy provides multiple **formats optimized for operations and construction**.

---

Agar chaho, main **ek visual cheat sheet bana doon jisme sparse formats (CSR, CSC, COO, DOK) + example matrix + memory saving illustration** dikh raha ho, jisse **instant understanding** mile.

Chahte ho main wo bana doon?


Perfect! Ab hum **NumPy aur Python me Images ke saath kaam karna** detail me samjhenge. Ye concept **image processing, computer vision, ML, and deep learning** ke liye bohot important hai.

---

## **1. Images as Arrays**

* Image = **2D or 3D array**

  * **Grayscale Image** → 2D array (height × width)
  * **Color Image (RGB)** → 3D array (height × width × 3)
  * **RGBA** → 3D array (height × width × 4)

* Each element → pixel intensity (0–255 for 8-bit images)

```python id="img1"
import numpy as np
from matplotlib import pyplot as plt
from PIL import Image

# Load image
img = Image.open("sample.jpg")
img_arr = np.array(img)
print(img_arr.shape)  # e.g., (height, width, 3) for RGB
```

---

## **2. Displaying Images**

```python id="img2"
plt.imshow(img_arr)
plt.axis('off')
plt.show()
```

* **Grayscale:** `plt.imshow(img_arr, cmap='gray')`

---

## **3. Image Manipulation with NumPy**

### **3.1 Accessing Pixels**

```python id="img3"
pixel = img_arr[100, 50]       # pixel at row=100, col=50
print(pixel)                   # RGB values e.g., [255 128 64]
```

---

### **3.2 Cropping an Image**

```python id="img4"
cropped = img_arr[50:200, 100:300]  # height 50-200, width 100-300
plt.imshow(cropped)
plt.axis('off')
plt.show()
```

---

### **3.3 Changing Pixel Values**

```python id="img5"
img_arr[0:50, 0:50] = 255  # Top-left 50x50 region white
plt.imshow(img_arr)
plt.show()
```

---

### **3.4 Converting to Grayscale**

```python id="img6"
gray = np.mean(img_arr, axis=2).astype(np.uint8)  # average over RGB channels
plt.imshow(gray, cmap='gray')
plt.axis('off')
plt.show()
```

* Other methods: weighted sum → `0.2989 R + 0.5870 G + 0.1140 B`

---

### **3.5 Flipping / Rotating**

```python id="img7"
# Flip vertically
flipped = np.flipud(img_arr)
plt.imshow(flipped)
plt.show()

# Flip horizontally
flipped_h = np.fliplr(img_arr)
plt.imshow(flipped_h)
plt.show()

# Rotate 90 degrees
rotated = np.rot90(img_arr)
plt.imshow(rotated)
plt.show()
```

---

### **3.6 Resizing Image**

* NumPy alone → not efficient
* Use **PIL / OpenCV**:

```python id="img8"
from PIL import Image

img = Image.open("sample.jpg")
resized = img.resize((200, 300))  # width=200, height=300
plt.imshow(resized)
plt.axis('off')
plt.show()
```

---

## **4. Image Arithmetic (NumPy Vectorized)**

* Brightness adjustment: `img_arr + 50` → add value to all pixels
* Contrast adjustment: `img_arr * 1.2` → multiply all pixels

```python id="img9"
bright = np.clip(img_arr + 50, 0, 255)  # clip to valid range
plt.imshow(bright)
plt.axis('off')
plt.show()
```

* `np.clip()` → ensures pixel values remain 0–255

---

## **5. Converting Image Back to PIL for Saving**

```python id="img10"
new_img = Image.fromarray(img_arr.astype(np.uint8))
new_img.save("output.jpg")
```

---

## **6. Tips for Working with Images**

1. **Always check shape** → RGB/Grayscale difference
2. **Use vectorized NumPy operations** → faster pixel manipulations
3. **Use PIL / OpenCV** for resizing, reading, writing
4. **Clipping values** → avoid overflow when doing arithmetic
5. **For ML/DL** → normalize pixel values (0–1) → `img_arr / 255.0`

---

💡 **Conclusion:**
Images in Python = **NumPy arrays**, jisse aap **read, display, manipulate, and save** kar sakte ho efficiently. Vectorized operations aur PIL/OpenCV ka combination **high-performance image processing** ke liye best hai.

---

Agar chaho, main **ek visual cheat sheet bana doon jisme image array → grayscale, crop, flip, rotate, brightness/contrast adjustment** ke examples ek diagram me dikh rahe ho, jisse **instant understanding** mile.

Chahte ho main wo bana doon?
