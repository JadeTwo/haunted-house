# The Haunted House

---

## Part 1: Ghosts!

The Ghosts are so strong… they have their own components! Create a `Light` component to even the playing field.

1. Create a `Light` component.
2. Remove the `img` tag in the `Bedroom`, `Kitchen`, `Bathroom`, and `Closet`, render the `Light` component instead.
3. The `Light` component should return the exact same `img` tag it's replacing.
4. Pass the `Light` component any props (data from the parent) it needs.

> **Progress Check:** Every room light should still be functional. For now, the lights should randomly turn off.

---

## Part 2: Let There Be Light!

This is hard work turning on all these lights… hook up the `SmartBulb` by lifting state to the `HauntedHouse` component.

5. Replace the local variable `light` in the `HauntedHouse` component with state that is identical to the one found in the `Bedroom` component.
6. Remove all state from `Bedroom`, `Kitchen`, `Bathroom`, and `Closet`.
7. Pass down the state and setter function from `HauntedHouse` to the `Bedroom`, `Kitchen`, `Bathroom`, and `Closet` components as props.
8. Pass down the setter function from `HauntedHouse` to the `SmartBulb` component.
9. Destructure the props in the child components so they can be used and remain functional.

> **Progress Check:** Clicking one light should turn on all lights in every room. The lights will still turn off randomly.

---

## Part 3: The Closet

They still don’t stay on… and this `SmartBulb` is broken! Yoink a new light bulb from the `Closet` to fix the main `SmartBulb` of the Haunted House using inverse data flow.

10. Pass the `yoink` function from `HauntedHouse` down through `Bedroom` $\rightarrow$ `Closet` $\rightarrow$ `Drawer` as props.
11. Inside `Drawer`, call `yoink` and pass it `newLightBulb` from inside the `open` function.
12. Inside `HauntedHouse`, call the setter function and pass it `bulb` from inside the `yoink` function.
13. Click on the secret drawer in the closet.

> **Progress Check:** The light bulb next to the words **"Haunted House"** should no longer be broken.

---

## Part 4 (Final): Here Goes Nothing...

14. Click the light bulb next to the words **"Haunted House"**.