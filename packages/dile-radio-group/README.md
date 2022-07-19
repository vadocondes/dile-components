# @dile/dile-radio-group

Web Components to create a customizable radio buttons interface. 

There are two components in this package:

- ```dile-radio-group```: allows to create a group of radio buttons. In a group only is possible to select one radio button at same time.
- ```dile-radio```: to create each radio button on the group

## Installation
```bash
npm i @dile/dile-radio-group
```

## Usage
```html
<script type="module">
  import '@dile/dile-radio-group/dile-radio-group.js';
  import '@dile/dile-radio-group/dile-radio.js';
</script>

<dile-radio-group name="interested" label="Are you interested in this subject?">
  <dile-radio label="Yes" value="yes"></dile-radio>
  <dile-radio label="Some interested" value="some"></dile-radio>
  <dile-radio label="Not at all" value="not"></dile-radio>
</dile-radio-group>
```

## Properties

### For dile-radio-group component

- **disabled**: The radio buttons are disabled.
- **name**: element name
- **label**: Text label for the group
- **value**: The selected radio value

### For dile-radio-group component

- **selected**: Boolean, true if its selected
- **label**: label for the radio element
- **value**: value for this radio element

## dile-radio-group custom events 

### element-changed

The ```element-changed``` event is dispatched when value on the input changes. 
In the event detail will emmit the element ```name``` and ```value```properties.

### dile-radio-group-changed

Is dispatched when the value changes.
In the event detail will emmit the element ```name``` and ```value```properties.

## dile-radio custom events 

### dile-radio-selected

New radio button selected. In this event the detail object only contains ```value``` property.

## CSS Custom Properties

Custom property | Description | Default
----------------|-------------|---------
--dile-input-label-font-size | Font size for the label | 1em
--dile-input-label-color | Color for the label text | #59e
--dile-input-label-font-weight | Label text font weight | normal
--dile-input-label-margin-bottom | Label marging bottom | 4px
--dile-radio-disabled-icon-color | Color for the icon when it is disabled | #ccc
--dile-radio-space-between-label-and-icon | Separation label on radios | 0.4rem
--dile-radio-icon-size | Radio icon size | 1.2rem
--dile-radio-icon-color | Radio icon color | #303030
--dile-radio-label-font-size | Radio label text size | 1rem
--dile-radio-label-color | Radio label text color | #303030
--dile-radio-selected-icon-color | Radio icon color | --dile-radio-icon-color or #303030
--dile-radio-selected-label-color | Radio label selected text color | --dile-radio-label-color or #303030