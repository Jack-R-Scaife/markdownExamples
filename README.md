# Markdown Examples

# Heading 1
## Heading 2
### Heading 3

---

## Bullet points
- One
- Two
    - Nested
- Three

## Numbered List
1. One
2. Two
     1. Nested
3. Three

## Checklists
- [ ] One
- [ ] Uncompleted
     - [ ] Nested
- [x] Completed

## Seperators
---
***
___

## Tables
 | Column 1 | Right Aligned | Centre Aligned |
 | --- | ---: | :---: |
 | Universe | 42 | Hitchhicker |
 | Data | 6060 | Lorem Ipsum |
 | Data | 987789 | Lorem Ipsum |

## Code Highlighting
- Code can be `highlighted inline` or in blocks:
```C++
#include <iostream>
void main()
{
	std::cout << "Hello World\n";
}
```

## Gantt Chart
```mermaid
gantt
    dateFormat  YYYY-MM-DD
    title       Example project gantt chart
    excludes    weekends
    %% (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)

    section Design
    Completed task            :done,    des1, 2023-09-25, 2d
    Active task               :active,  des2, 2023-09-27, 2d
    Future task               :         des3, after des2, 5d
    Future task 2             :         des4, after des3, 5d

    section Implementation
    Completed critical task             :crit, done, 2023-10-10, 60h
    Active critical task                :crit, active, after des1, 3d
    Critical future task                :crit, 5d
    Future task 3                       :3d
    Future task 4                       :4d
    Implementation done                 :milestone, 2023-10-20, 0d

    section Documentation
    Future task 5                       :active, a1, after des1, 3d
    Add gantt diagram to demo page      :after a1  , 4d
```

## Whole Examples
- [weekly minutes example](weekly%20minutes%20example.md)
- [weekly log example](weekly%20log%20example.md)  

I also created a couple of templates if anyone wishes to use them:  
- [weekly minutes template](weekly%20minutes%20template.md)  
- [weekly log template](weekly%20log%20template.md)