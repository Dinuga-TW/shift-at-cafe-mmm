# Shift at Cafe Mmm

A small first-person café simulation I made for university using Unity.

The idea is quite simple: you work a shift at a café, talk to customers, seat them, take their orders, wait for the food to be prepared, serve them and take payment. Each customer has their own dialogue, order and animations, while the game keeps track of things like available stock, customers served and the day's income.

## Gameplay

Customers arrive one at a time and can be spoken to and interacted with, using the first-person interaction system. After finding out what they want, they can be assigned a seat using the in-game iPad.

So, the player can essentially:

* Seat customers at available tables
* Place orders through the iPad
* View order prices and preparation times
* Keep track of active orders
* Pick up prepared food and drinks
* Serve the customer
* Take payment after they finish
* Track stock, customers served and daily income

The main customers have their own dialogue, orders and animation states, including talking, sitting, eating and drinking.

## Controls

The project uses an on-screen first-person controller for camera control.

* **Movement control (WASD)** — Move around the environment
* **Look control (eye icon)** — Click and drag to look around
* **Left Click** — Interact with customers, food and UI elements
* **Tab** — Show/hide the iPad
* **Esc** — Pause menu

## Character Animation

Character animation workflow was one of the bigger parts of the project. 

The character models and animations were sourced from Mixamo, then taken through MotionBuilder for setup, control rig work, animation processing, and then for preparing the animation clips for use in Unity.

Once imported to Unity, the animations were connected to Animator Controllers and state-based logic, allowing each customer to switch between different actions depending on what they were doing in the game.

## Implementation

Most of the gameplay systems were put together using Unity Visual Scripting, including the customer interactions, dialogue, ordering system, cooking timers, UI updates, inventory and payment flow. The first-person controller was one of the core coursework requirements and became the basis for moving around and interacting with the café.

The project also uses prefabs for characters and interactive objects, an in-game iPad UI for managing the café, and first-person raycast interaction for dealing with customers and orders.

Outside the main gameplay loop, I also spent some time building out the setting with a beach environment, water, sunset lighting, ambient audio, music and a few smaller details like a video playing on the café TV.

## Playable Build

A Windows build of the project is available here:

**[Download Windows Build](https://drive.google.com/file/d/1mMNB70w9DuZikhBcz-5XozGKznkJajDv/view?usp=sharing)**

To run it:

1. Download `Shift-at-Cafe-Mmm-Windows.zip`
2. Extract the ZIP somewhere on your PC
3. Open the extracted folder
4. Run `Shift at Cafe Mmm.exe`

**Note:** Google Drive may show a warning that it can't scan the ZIP for viruses because of the file size. Nothing sketchy in there, Drive just has a pretty low scan limit, so it is safe to download. Download size: **~180 MB**

## Project Showcase

A short showcase of the project, covering the main gameplay loop, a few cinematic shots, and a very brief look at the MotionBuilder animation work and Unity Visual Scripting.

**[Watch the Project Showcase](https://youtu.be/N0ri1gpJVpE)**


## Project Notes

This originally started from the practical/tutorial work provided for the university module and was expanded into the final café simulation.

Some of the environment, character and animation assets were provided by the module or sourced from places such as Mixamo and the Unity Asset Store. The main focus of my work was putting those pieces together into the final interactive experience, including the animation pipeline, customer interactions, dialogue, ordering, UI, inventory and other gameplay systems.

There are definitely a few rough edges and it’s not the most complex project. It was also built within the scope of a university module in mind rather than as a full-blown café simulation. I did push it further than the minimum requirements though, and there is still plenty here that could be expanded into something much bigger if I ever decide to revisit the idea. And maybe one day I will.

## Built With

* Unity 2022.3
* Autodesk MotionBuilder
* Mixamo
* C#
