# Uncommon Tailwind CSS Bug: Invalid Class Names

This repository demonstrates an uncommon bug in Tailwind CSS where misspelled or invalid class names result in unexpected or missing styling. The bug is subtle and can be difficult to track down because it usually doesn't throw JavaScript errors.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe that the text does not have the expected styling because of invalid class names in `SomeTailwindComponent.js`.

## Solution

The solution, shown in `SomeTailwindComponentSolution.js`, involves carefully checking all Tailwind CSS class names used in the component for typos and ensuring they are correctly defined in the `tailwind.config.js` file or are generated based on your Tailwind configuration.

## Lessons Learned

- Always double-check your Tailwind CSS class names for typos.
- Regularly clean up unused CSS classes to improve readability and reduce the risk of errors.
- Using a linter can help catch invalid class names before they become a problem. Consider using a linter such as ESLint with a Tailwind CSS plugin.