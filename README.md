# Tailwind CSS @apply Inheritence Problem

This repository demonstrates an uncommon bug related to Tailwind CSS's `@apply` directive.  The bug manifests when using `@apply` within a component's style attribute, causing inconsistent or missing styles, primarily in nested scenarios. The `@apply` directive doesn't consistently inherit or cascade styles as expected in this context.

## Bug Reproduction

The `bug.html` file showcases the problematic code. You can observe that the inner `div` sometimes fails to inherit the expected styles (background color and rounded corners) applied through the `@apply` directive.

## Solution

The `bugSolution.html` file provides a workaround.  The recommended solution involves separating the styles into dedicated classes and applying them directly to the elements, ensuring proper inheritance and style cascade.