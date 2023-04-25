---
theme: seriph
---


# Slide 1

Content of my slide

---

# Slide 2

Union Types in TypeScript

```ts
const log = (arg: any) => console.log(arg);

let age: number | string;

age = 26;
log(age); // 26

age = "26";
log(age); // '26'
```

---

# Animations

Subtitle

<v-click>

Text to animate

</v-click>

<div v-click>Hello, World!</div>
<div v-after>After</div>

<v-clicks>

- Item 1
- Item 2
- Item 3
- Item 4

</v-clicks>

<div v-click="3">1</div>
<div v-click="2">2</div>
<div v-click="1">3</div>

<style>
.slidev-vclick-target {
    transition: all 2000ms ease 10ms;
}

.slidev-vclick-hidden {
    transition: scale(0)
}
</style>

---
preload: false
---

# Motion

<div
    v-motion
    :initial="{ x: 80, y: 80, opacity: 0 }"
    :enter="{ x: 0, y: 0, opacity: 1, transition: {
        type: 'spring',
        damping: 10,
        stiffness: 20,
        mass: 4,
        delay: 1000,
        duration: 2000
    } }">
    <img src="images/awesome.jpg" style="margin: auto; width: 80%" />
</div>
