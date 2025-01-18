# JavaScript Null Check Bug with Type Coercion

This repository demonstrates a common yet subtle bug in JavaScript related to null checks and type coercion. The bug arises from a naive null check that doesn't consider potential type coercion issues.

## Bug Description

The `foo` function is designed to add two numbers. However, it incorrectly handles null values by immediately returning null, without attempting type coercion. This leads to unexpected results when one or both inputs are null.

## Bug Solution

The solution involves employing stricter null checks and handling type coercion appropriately.  We'll use the loose equality operator (`==`) to handle type coercion and ensure the inputs are numbers before adding them.  If a null or undefined value is provided, it is converted to 0.