# Project 1 - *Wordle Pt. 1*

Submitted by: **Rohit Biswas**

**Wordle** is a daily word puzzle game where players have six attempts to guess a hidden five-letter word. 

Time spent: **4** hours spent in total

## Required Features

The following **required** functionality is completed:

- [X] App displays a keyboard on the screen
- [X] When tapping on the keyboard, a letter is shown or deleted (letter selected)
- [X] User can play a basic version of Wordle, with different goal words each time

The following **optional** features are implemented:

- [ ] Improve and customize the user interface by adding a launch screen and app icon
- [ ] Run the app on a device rather than in the simulator

## Video Walkthrough

<div style="position: relative; padding-bottom: 192.17081850533808%; height: 0;">
  <iframe src="https://www.loom.com/embed/5ae35495b8a14d37b97f4442bde858c8?sid=2a3f0f4b-45fb-44db-8fd1-246988e255b6" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
</div>


## Notes

# Challenges Encountered

During the development of this Wordle clone, several challenges arose:

- **Keyboard Input Mapping:**  
  Handling keyboard inputs and ensuring that each tap correctly updates the corresponding cell in the collection view was tricky. Managing closures and delegate methods to propagate these events required careful attention.

- **UICollectionView Cell Reuse:**  
  Since cells are reused, maintaining the correct state (e.g., clearing letters and resetting styles) when a cell is dequeued was challenging. Ensuring that outdated data wasn't displayed involved fine-tuning cell lifecycle management.

- **Animation Synchronization:**  
  Implementing smooth animations—such as scaling a cell upon letter entry—necessitated carefully configuring animation blocks and completion handlers. Resetting the transformation properly after animations was essential for a polished user experience.

- **Game Logic Complexity:**  
  Detailed state management involves determining whether a letter is correct but in the wrong position or perfectly correct. A key challenge was ensuring this logic worked flawlessly with the UI feedback (color coding).

- **UI Styling and Color Management:**  
  Applying dynamic styles to cells based on game state, especially converting between `UIColor` and `CGColor` for border styling, required a meticulous approach to ensure consistency and visual clarity across different devices.

## License

    Copyright 2025 Rohit Biswas

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
