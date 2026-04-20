C++ HalfGammon Game with Undo Feature
Overview

This project is a console-based implementation of a simplified backgammon-style game called HalfGammon, developed in C++. The game allows two players to take turns moving pieces while maintaining an accurate and dynamic game state.

A key feature of this project is the implementation of an undo system, which allows players to revert previous moves. This functionality is powered by a custom-built stack using a linked list instead of standard library data structures.

The purpose of this project was to strengthen understanding of data structures, dynamic memory management, and state tracking in an interactive application.

Features
Turn-based two-player gameplay
Console-based board display with clear formatting
Move validation to prevent illegal actions
Undo functionality supporting multiple consecutive undos
Custom stack implementation using a linked list (LIFO structure)
Dynamic memory management using new and delete
Continuous game state updates after each move
Tech Stack
Language: C++
Concepts:
Linked Lists
Stack (custom implementation)
Dynamic Memory Allocation
Functions and modular programming
Game state management
Tools:
zyBooks IDE or standard C++ compiler
How It Works

The game board is updated after each player move. Each move stores a snapshot of the game state, which is pushed onto a custom stack.

When a player selects undo:

The most recent game state is popped from the stack
The board is restored to the previous configuration
The turn is reverted

This ensures consistent and reliable state restoration.

Development Process
Designed the HalfGammon board and rules
Implemented core gameplay mechanics (movement and turns)
Built the board display system
Created a linked list node structure
Implemented stack operations (push and pop)
Integrated undo functionality into the game loop
Added input validation and error handling
Tested gameplay and undo behavior
Debugged memory and pointer-related issues
Challenges
Implementing a reliable undo system that restores full game state
Managing dynamic memory safely and avoiding leaks
Debugging pointer-related errors
Handling edge cases such as undo at the start of the game
Maintaining modular code without using standard library containers
