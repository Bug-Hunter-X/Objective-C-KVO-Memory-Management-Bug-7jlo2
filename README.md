# Objective-C KVO Memory Management Bug

This repository demonstrates a common yet subtle bug in Objective-C related to Key-Value Observing (KVO) and memory management.  The bug occurs when observers are not properly removed, leading to potential crashes or unexpected behavior when the observed object is deallocated.

The `bug.m` file contains the buggy code, while `bugSolution.m` provides the corrected implementation.  The key to fixing this issue is to remove observers in the `-dealloc` method or using appropriate blocks with automatic cleanup.

## Setup

1. Clone this repository.
2. Open the project in Xcode.
3. Run the code to observe the bug and solution.