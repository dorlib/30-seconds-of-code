---
title: getAgeByDate
tags: Date
expertise: begginer
firstSeen: 2022-07-22T05:00:00-04:00
---

- Get age by given date with the following format: "DD.MM.YYYY".
- `getAgt()` stores an int which represents the age.
- Use `Date(birthDate).getTime()` method to return the numeric value corresponding to the time for the specified date according to universal time.
- Use `(new Date() - new Date(birthDate).getTime())` to get the time passed in miliseconds.
- Eventually Use `/ 3.15576e+10` and `Math.floor()` to get the desired age.

```js
    let birthDate = "DD.MM.YYYY" 
    const getAge = birthDate => Math.floor((new Date() - new Date(birthDate).getTime()) / 3.15576e+10)
```

```js
getAge('11.11.2000'); // 21
getAge('11.11.2000'); // 62
```
