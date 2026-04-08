Software developer focused on systems, game development, and applied machine learning.

---
```cpp
float Q_rsqrt( float number )
{
	long i;
	float x2, y;
	const float threehalfs = 1.5F;

	x2 = number * 0.5F;
	y  = number;
	i  = * ( long * ) &y;                       // evil floating point bit level hacking
	i  = 0x5f3759df - ( i >> 1 );               // what the #&$*?
	y  = * ( float * ) &i;
	y  = y * ( threehalfs - ( x2 * y * y ) );   // 1st iteration
//	y  = y * ( threehalfs - ( x2 * y * y ) );   // 2nd iteration, this can be removed

	return y;
}
```
## Tech Stack
### Languages
![C++](https://img.shields.io/badge/C++-informational?style=flat\&logo=c%2B%2B\&logoColor=white)
![C#](https://img.shields.io/badge/C%23-informational?style=flat\&logo=c-sharp\&logoColor=white)
![Python](https://img.shields.io/badge/Python-informational?style=flat\&logo=python\&logoColor=white)

### Tools & Engines
![Unity](https://img.shields.io/badge/Unity-informational?style=flat\&logo=unity\&logoColor=white)
![Godot](https://img.shields.io/badge/Godot-informational?style=flat\&logo=godot-engine\&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-informational?style=flat\&logo=linux\&logoColor=white)

---
## About

* Currently working on:

  * Card game (Godot)
  * FPS prototype (Godot)
  * Puzzle platformer (Godot)
  * Library management system
  * Conversation classifier

* Currently learning:

  * Multiplayer architecture
---

