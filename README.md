```markdown

The feature based approach 
for structuring a large
react native app

root/
│
├─── package.json
├─── tsconfig.json
├─── .gitignore
├─── index.ts
│
└─── src/
     │
     ├─── auth/
     │     ├─── components/
     │     │      └─── LoginButton.tsx
     │     ├─── services/
     │     │      └─── AuthService.ts
     │     ├─── screens/
     │     │      └─── LoginScreen.tsx
     │
     ├─── profile/
     │     ├─── components/
     │     │      └─── ProfilePicture.tsx
     │     ├─── services/
     │     │      └─── ProfileService.ts
     │     ├─── screens/
     │     │      └─── ProfileScreen.tsx
     │
     ├─── shared/
     │     ├─── components/
     │     │      └─── Header.tsx
     │     ├─── utils/
     │     │      └─── helpers.ts
     │     └─── config/
     │            └─── config.ts
  App.tsx


```




```markdown

Typical React Native app 
structured by layer.

root/
│
├─── package.json
├─── tsconfig.json
├─── .gitignore
├─── index.ts
│
└─── src/
     │
     ├─── App.tsx
     │
     ├─── components/
     │     └─── Button.tsx
     │
     ├─── screens/
     │     └─── HomeScreen.tsx
     │
     ├─── services/
     │     └─── AuthService.ts
     │
     ├─── models/
     │     └─── UserModel.ts
     │
     ├─── utils/
     │     └─── Helpers.ts
     │
     └─── config/
           └─── config.ts

```



```javascript




// The Spread Operator

// You can merge all items from a list 
// into another list using ...
const array = [1, 2, 3]
const array2 = [...array, 4, 5, 6]
console.log(array2) 
// -> [1, 2, 3, 4, 5, 6]

// You can spread objects 
// into others the same way
const obj = {prop: 1, prop2: 2}
const obj2 = {...obj, prop3: 3}
console.log(obj2) 
// -> {prop: 1, prop2: 2, prop3: 3}

// You can use the spread operator even 
// in functions parameters, to pass 
// an unlimited amount of parameter 
// to the function 
function foo(...args){
  // the args will be passed as array
  // containing all items you passed as
  // parameter
  console.log(args)
}
foo(1, 2, 3) // -> [1, 2, 3]




```

```css

.polymorphism-text {
  font-family: 'Arial', sans-serif; 
  font-size: 40px; 
  color: #e1e1e1; 
  font-weight: bold; 
  text-shadow: 
  1px 1px 2px rgba(0, 0, 0, 0.2), 
  -1px -1px 2px rgba(255, 255, 255, 0.7); 
  text-transform: uppercase; 
  letter-spacing: 5px;  
}
```

```html

<div 
  class="polymorphism-container"
  >
    <span 
      class="polymorphism-text"
    >
      POLYMORPHISM
    </span>
</div>

```

```python
# For Loop
for i in range(5):
    print(f"Iteration {i}")

# While Loop
count = 0
while count < 5:
    print(f"Count is {count}")
    count += 1
```

```python

```

```python
# Working with Lists
fruits = ["apple", "banana", "cherry"]
fruits.append("orange")  # Add an item
print(fruits[1])  # Access an item

for fruit in fruits:
    print(fruit)
```
























