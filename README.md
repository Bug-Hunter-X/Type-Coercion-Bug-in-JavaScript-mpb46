# Type Coercion Bug in Javascript

This repository demonstrates a common, yet subtle, bug in JavaScript related to type coercion. The bug arises from using loose equality (==) instead of strict equality (===). Loose equality performs type coercion before comparison, while strict equality does not. This difference can lead to unexpected behavior and logic errors.

## Bug Description
The JavaScript function `foo` adds two numbers. It handles `null` input values correctly when using the strict equality operator (`===`).  However, if you replace `===` with `==`, unexpected results arise from Javascript's automatic type conversion.