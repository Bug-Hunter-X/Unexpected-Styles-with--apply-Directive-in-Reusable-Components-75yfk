# Unexpected Styles with @apply Directive in Reusable Components

This repository demonstrates a bug related to Tailwind CSS's `@apply` directive when used within reusable components.  The `@apply` directive, while convenient, does not re-evaluate styles based on component props or state if the component is rendered multiple times. This can result in unexpected visual discrepancies or incorrect styling.

## Reproduction

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Observe the inconsistencies in styling across multiple instances of the component.

## Solution

The solution involves replacing `@apply` with explicit utility classes or creating a dynamic utility class based on props. This ensures the correct styles are applied for each component instance.

## How to Contribute

Feel free to open an issue if you find any additional bugs or have suggestions for improvement.