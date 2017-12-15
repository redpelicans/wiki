<!-- TITLE: Recruiting -->
<!-- SUBTITLE: A quick summary of Recruiting -->

# technical interview

## factorial
```javascript
// es6 function syntax
const f1 = () => {};

// map definition
// iteratee signature: (item, index|key)
// always return a collection with the same size
const f2 = (n) => n*2;
const a1 = [1,2,3];
const f3 = _.map(a1, f2);

// what will be f3(a1) ?
console.log(a1, f3(a1));

// exercice: i want [4,5,6]

// reduce definition -> map with a state (memo)
// iteratee signature: (memo, item, index|key)
const f4 = (memo, n) => n*2;
const f5 = _.reduce(a1, f4, 0);

// what will be f4(a1) ?
console.log(a1, f4(a1));

// exercice: i want 4! (1x2x3x4 = 24)
// exercice: i want [1,3] from a1 (reject even number)
```

## analog watch

```javascript
// 1a- use _.times to display an array of 4 0 in the console [0,0,0,0]
const ex1a = _.times(4, _.constant(0));
// 1c- create a function to parameterize the length
const ex1b = (l) => _.times(l, _.constant(0));
// 1d- use an iterator (no _.constant)
const ex1c = (l) => _.times(l, () => 0);
console.log(ex1a, ex1b(4), ex1c(4));

// 2a- use reduce to display an array in the console with a 1 [1,0,0,0]
const ex2a = _.reduce(
  ex1b(4),
  (memo, i, index) => ([...memo, index === 0 ? 1 : 0]),
  []
);
// 2b- create a function to parameterize the length and the position of 1
const ex2b = (l, p) => _.reduce(
  ex1b(l),
  (memo, i, index) => ([...memo, p === index ? 1 : 0]),
  []
);
// 2c- update the previous function to have
// [*,0,0]
// [0,*,0]
// [0,0,*]
const ex2c = (l, p, symbol) => _.reduce(
  ex1b(l),
  (memo, i, index) => ([...memo, p === index ? symbol : 0]),
  []
);
console.log(ex2a, ex2b(4, 2), ex2b(3, 0, '*'), ex2b(3, 1, '*'), ex2b(3, 2, '*'));

// bonus: create a generic function to have 2c for any length
//console.log(bonus(4, '-'))
// [-,0,0,0]
// [0,-,0,0]
// [0,0,-,0]
// [0,0,0,-]
```

## arithmetic suite

```javascript
// arithmetic suite -> accumulator
const acc = _.reduce(
  [0,1,2,3],
  (memo, i) => memo + i,
  0
);

// arithmetic suite -> accumulator parameterized (length)
const accp = (l) => _.reduce(
  _.range(l),
  (memo, i) => memo + i,
  0
);

// arithmetic suite -> accumulator parameterized (length, start)
// you! (2 ways)

// arithmetic suite -> accumulator parameterized (length, start, exclusion)
const accpex = (l, start, exc) => _.reduce(
  _.range(l),
  (memo, i) => i === exc ? memo : memo + i,
  start
);

// arithmetic suite -> accumulator parameterized (length, start, max)
// you!

console.log(acc, accp(5), accpex(5, 0, 3), accpex(5, 3, 3));

// store 10 accumulations in an array with a map
// groupby accumulations: >=10, >=50, <50
// get the most numerous group of accumulations
// you!
```
