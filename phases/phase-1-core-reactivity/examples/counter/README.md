# Counter Example - Demonstrating Reactivity

## Simple Counter
```hjx
component Counter

state:
  count = 0

computed:
  doubled = count * 2
  isEven = count % 2 === 0

layout:
  view:
    text: "Count: {{count}}"
    text: "Doubled: {{doubled}}"
    text: "Is even? {{isEven}}"
    
    button(on click -> increment): "+"
    button(on click -> decrement): "-"
    button(on click -> reset): "Reset"

handlers:
  increment:
    set count++
  
  decrement:
    set count--
  
  reset:
    set count = 0

```
 # Key Features Demonstrated

 1. Signal tracking - Only the text showing count updates

 2. Computed values - doubled and isEven update automatically

 3. Direct mutations - count++ works naturally
