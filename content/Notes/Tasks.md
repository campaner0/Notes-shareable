---
type: note
---


## To Do Today
```tasks
due today
not done
heading does not include Tasks
```





---

## Due This Week
```dataviewjs
const query = `
not done
due before in 7 days
path does not include ${dv.current().file.path}
`;

dv.paragraph('```tasks\n' + query + '\n```');
```



---


## Due in the Future
```tasks
not done
due after in 7 days
```



---

## Done Today
```tasks
done today
```


