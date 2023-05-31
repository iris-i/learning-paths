---
title: 'TIL: How to isolate the first item in an array and return the rest.'
status: 'published'
author:
  name: 'Iris Ibekwe'
  picture: 'https://avatars.githubusercontent.com/u/5355315?v=4'
slug: 'til-how-to-isolate-the-first-item-in-an-array-and-return-the-rest'
description: ''
coverImage: ''
category: [{"label":"ES6","value":"es6"},{"label":"Javascript","value":"javascript"}]
learningPath: ''
publishedAt: '2023-05-01T22:57:25.000Z'
---

You can use the destructuring assignment to get values from Javascript arrays and or properties from objects into variables.

Eg. To return the first item in a list of upcoming events:

```
let events = [
   {
    title: 'swim',
      month: 'January',
    },
    {
      title: 'volleyball',
      month: 'February',
    },
    {
      title: 'prom',
      month: 'May',
    },
  ]
```

Destructuring the events array will return 2 lists of events:

```
const[nearestEvent, ...restOfEvents] = events
// console.log(NearestEvent) returns the first item in the list:
{title: 'swim', month: 'January'}

// console.log(restOfEvents) returns the remaining items.
0: {title: 'volleyball', month: 'February'}
1: {title: 'prom', month: 'May'}
```

