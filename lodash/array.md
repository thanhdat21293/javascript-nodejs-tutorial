
## Array

#### Chunk

Tạo một mảng các phần tử chia thành các nhóm theo chiều dài của kích thước. Nếu mảng không thể được chia đều, phần cuối cùng sẽ là các phần tử còn lại.

```javascript
_.chunk(array, size)
```

VD:

```javascript
_.chunk(['a', 'b', 'c', 'd'], 2);
// => [['a', 'b'], ['c', 'd']]
 
_.chunk(['a', 'b', 'c', 'd'], 3);
// => [['a', 'b', 'c'], ['d']]
```

#### Compact

Tạo ra một mảng với tất cả các giá trị falsey gỡ bỏ. Các giá trị false, null, 0, "", undefined, và NaN là falsey.

```javascript
_.compact(array)
```

VD:
```javascript
_.compact([0, 1, false, 2, '', 3]);
// => [1, 2, 3]
```

#### Concat

Tạo một mảng kết hợp mảng mới với bất kỳ mảng bổ sung và / hoặc các giá trị.

```javascript
_.concat(array, [values])
```

VD: 

```javascript
var array = [1];
var other = _.concat(array, 2, [3], [[4]]);
 
console.log(other);
// => [1, 2, 3, [4]]
 
console.log(array);
// => [1]
```

#### Drop

Xóa n phần tử trong mảng bắt đầu từ phần tử đầu tiên trong mảng.

```javascript
_.drop(array, [n=1])
```

VD: 

```javascript
_.drop([1, 2, 3]);
// => [2, 3]
 
_.drop([1, 2, 3], 2);
// => [3]
 
_.drop([1, 2, 3], 5);
// => []
 
_.drop([1, 2, 3], 0);
// => [1, 2, 3]
```

#### DropRight

Xóa n phần tử trong mảng bắt đầu từ phần tử cuối cùng trong mảng.

```javascript
_.dropRight(array, [n=1])
```

VD: 

```javascript
_.dropRight([1, 2, 3]);
// => [1, 2]
 
_.dropRight([1, 2, 3], 2);
// => [1]
 
_.dropRight([1, 2, 3], 5);
// => []
 
_.dropRight([1, 2, 3], 0);
// => [1, 2, 3]
```

#### Fill

Thay thế các phần tử của mảng có giá trị từ khi bắt đầu đến kết thúc, không bao gồm phần tử cuối.

```javascript
_.fill(array, value, [start=0], [end=array.length])
```

VD:

```javascript
var array = [1, 2, 3];
 
_.fill(array, 'a');
console.log(array);
// => ['a', 'a', 'a']
 
_.fill(Array(3), 2);
// => [2, 2, 2]
 
_.fill([4, 6, 8, 10], '*', 1, 3);
// => [4, '*', '*', 10]
```
#### FlattenDeep

Xử lý mảng lồng nhau thành một mảng.

```javascript
_.flattenDeep(array)
```

VD: 

```javascript
_.flattenDeep([1, [2, [3, [4]], 5]]);
// => [1, 2, 3, 4, 5]
```

#### FlattenDepth

Xử lý mảng lồng theo cấp độ.

```javascript
_.flattenDepth(array, [depth=1])
```

VD:

```javascript
var array = [1, [2, [3, [4]], 5]];
 
_.flattenDepth(array, 1);
// => [1, 2, [3, [4]], 5]
 
_.flattenDepth(array, 2);
// => [1, 2, 3, [4], 5]
```

#### FromPairs

Chuyển đổi từ mảng thành object

```javascript
_.fromPairs(pairs)
```

VD: 

```javascript
_.fromPairs([['a', 1], ['b', 2]]);
// => { 'a': 1, 'b': 2 }
```

