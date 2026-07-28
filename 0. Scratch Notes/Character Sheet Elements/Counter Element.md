The Counter Element is a tool designed to parse and display a numerical counter within Obsidian. It allows you to define a counter with customizable maximum and minimum values using YAML syntax, and then renders this information in an interactive format for easy tracking during gameplay or writing.

## Usage

[](https://github.com/SteelCompendium/draw-steel-elements/blob/main/docs/counter.md#usage)

To use the Counter Element, insert a code block with the language identifier `ds-counter` in your Obsidian note, and then define your counter using YAML syntax inside the code block.


```ds-counter
max_value: 20
current_value: 10
min_value: 0
name: Health
value_height: 3
name_height: 1
```

## Field Definitions

[](https://github.com/SteelCompendium/draw-steel-elements/blob/main/docs/counter.md#field-definitions)

Below is a detailed description of each field used in the counter element, including their types, default values, and whether they are required.

| Field           | Type      | Description                                                        | Required | Default Value |
| --------------- | --------- | ------------------------------------------------------------------ | -------- | ------------- |
| `name`          | `string`  | The name of the counter (e.g., "Health", "Mana").                  | **Yes**  | N/A           |
| `current_value` | `integer` | The current value of the counter.                                  | No       | `0`           |
| `max_value`     | `integer` | The maximum value the counter can reach.                           | No       | `undefined`   |
| `min_value`     | `integer` | The minimum value the counter can reach.                           | No       | `0`           |
| `value_height`  | `integer` | Adjusts the size of the counter value text in the rendered output. | No       | `3`           |
| `name_height`   | `integer` | Adjusts the size of the counter name text in the rendered output.  | No       | `1`           |


### Notes:

[](https://github.com/SteelCompendium/draw-steel-elements/blob/main/docs/counter.md#notes)

- The `current_value` is the starting point of the counter when it's rendered.
- If `max_value` is defined, the counter cannot increment beyond this value.
- If `min_value` is defined, the counter cannot decrement below this value.
- `value_height` and `name_height` are optional parameters to adjust the visual presentation of the counter in the rendered output. They are useful for customizing the display according to your preferences.
- You can click on the counter value to edit it directly.