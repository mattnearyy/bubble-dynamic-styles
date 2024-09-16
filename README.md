# How to Use Dynamic Icons in Bubble

## 1. Add a script to your app

- Go to SEO/Meta tags settings
- Paste the provided script in the header section
- **Note**: For free plans, add the script in an HTML element instead

## 2. Install the "Classify" plugin

- Install from [here](https://bubble.io/plugin/classify-1568299250417x684448291308175400).
- Ensure it's up to date. 

## 3. Update your data structure

- Add an "Icon" field (text type) to store icon names

## 4. In the Bubble editor

- Select the Icon element
- In the ID field, use Classify syntax:
  ```
  [setDynamicIcon('phosphor', '{icon label goes here}', '{icon fill type goes here}')]
  ```
- If the icon library does not have a fill option just omit this last argument, i.e. use:  ```[setIconDynamic(this, '{icon label}');]```
- Use lowercase for your icon label ('house' or 'users' etc) and fill types ('regular' or 'filled' etc). Use the value names that the library uses.

## 7. For conditional styling

- Duplicate the Classify syntax
- Modify parameters based on your conditions (e.g., change 'regular' to 'fill' when active)

## Other notes
- For Font Awesome 4, omit the 'fa' before the icon label.
