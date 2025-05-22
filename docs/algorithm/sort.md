# 排序算法

## 冒泡排序

```js
function bubbleSort(array) {
  if (!Array.isArray(array) || array.length <= 1) return array
  let lastIndex = array.length - 1
  while (lastIndex > 0) {
    let flag = true
    const k = lastIndex
    for (let j = 0; j < k; j++) {
      if (array[j] > array[j + 1]) {
        flag = false
        lastIndex = j
        ;[array[j], array[j + 1]] = [array[j + 1], array[j]]
      }
    }
    if (flag) break
  }
  return array
}

---

```
