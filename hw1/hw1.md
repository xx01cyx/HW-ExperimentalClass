Investigation in https://www.sjtu.edu.cn
========================================

Analyzation
-----------
* Offscreen pictures unnecessarily rendered.
* Redundant DOM elements.
* Huge network loads.

Optimizing Solutions
---------------------
* Postpone loading offscreen pictures.
* Use `{ passive: true }` (Passive Event Listeners) to improve the rolling performance of the website.
* Avoid using `document.write()`.
* Less DOM elements.
* More efficient web framework.