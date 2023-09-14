---
title: Collapse
lang: en-US
---

# Collapse

Use Collapse to store contents.

## Basic usage

You can expand multiple panels

:::demo

collapse/basic

:::

## Accordion

In accordion mode, only one panel can be expanded at once

:::demo Activate accordion mode using the `accordion` attribute.

collapse/accordion

:::

## Custom title

Besides using the `title` attribute, you can customize panel title with named slots, which makes adding custom content, e.g. icons, possible.

:::demo

collapse/customization

:::

## Collapse API

### Collapse Attributes

| Name                  | Description                        | Type                                                       | Default |
| --------------------- | ---------------------------------- | ---------------------------------------------------------- | ------- |
| model-value / v-model | currently active panel             | ^[string] (accordion mode) / ^[array] (non-accordion mode) | —       |
| accordion             | whether to activate accordion mode | ^[boolean]                                                 | false   |

### Collapse Events

| Name   | Description                        | Parameters                                                            |
| ------ | ---------------------------------- | --------------------------------------------------------------------- |
| change | triggers when active panels change | `(activeNames: array (non-accordion mode) / string (accordion mode))` |

### Collapse Slots

| Name    | Description               | Subtags       |
| ------- | ------------------------- | ------------- |
| default | customize default content | Collapse Item |

## Collapse Item API

### Collapse Item Attributes

| Name     | Description                        | Type                | Default |
| -------- | ---------------------------------- | ------------------- | ------- |
| name     | unique identification of the panel | ^[string]/^[number] | —       |
| title    | title of the panel                 | ^[string]           | —       |
| disabled | disable the collapse item          | ^[boolean]          | —       |

### Collapse Item Slot

| Name    | Description                    |
| ------- | ------------------------------ |
| default | content of Collapse Item       |
| title   | content of Collapse Item title |