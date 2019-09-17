## Stretch One
### Find the Treasure

```javascript
const treasureMap = [
  ['', '', ''],
  ['', '', 'X'],
  ['', '', ''],
];

const findTheTreasure = (map, treasure) => {

  // YOUR CODE
  for(let i=0; i<map.length; i++){
    for(let j=0; j<map[i].length; j++){
      let target=map[i][j];
      if(target===treasure){
        return [i,j];
      }
    }
  }
  return 'No treasure!';
};

findTheTreasure(treasureMap, 'X'); // => [2, 1]; (this is [x, y] - 0 indexed);
findTheTreasure(treasureMap, 'o'); // => 'No treasure!';
```
