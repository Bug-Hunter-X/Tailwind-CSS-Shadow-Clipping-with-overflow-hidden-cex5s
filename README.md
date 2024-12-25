# Tailwind CSS Shadow Clipping Bug

This repository demonstrates a subtle bug in Tailwind CSS where shadows are clipped when the parent element has `overflow-hidden` applied.  This can lead to unexpected visual results, especially when dealing with cards or other elements with shadows and potential content overflow.

## Bug Description

When an element with a shadow (e.g., using `shadow-md`) is a child of a parent element with `overflow-hidden`, the shadow can be clipped by the parent, resulting in an incomplete or truncated shadow.  This is not immediately apparent and can be difficult to debug.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe the shadow on the card.  Notice that the shadow is truncated, appearing incomplete.

## Solution

The solution involves using a wrapper element to contain the shadow. This workaround prevents the parent's `overflow-hidden` from interfering with the shadow rendering.

Check out `bugSolution.html` for a working example.

## Contributing

Contributions are welcome! If you have any other solutions or related issues, feel free to open a pull request.