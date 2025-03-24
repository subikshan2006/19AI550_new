# Ex.No: 4  Create a player Movement Script in unity 
### DATE: 24.3.2025                                                                           
### REGISTER NUMBER :212223240161
### AIM: 
To write a program to create a player movement in unity.
### Algorithm:
1. Create a New Unity Project by Open the  Unity Hub and create a new 3D Project,Name the project (e.g., PlayerMovement).
2. Create the Moving Object
   In the Hierarchy, right-click → 3D Object → Capsule (or Sphere).
   Rename it to Player 
4. Adding the Player Movement Behavior Script
   Create the Script-In the Project Window, go to the Assets folder.
   Right-click → Create → C# Script.
5. Write a script for player behavior and save it
6. Attach the Script
   Select player in the Hierarchy - Drag & Drop the playerBehavior script onto the Inspector Panel.
7. Run the game 
8. Stop the program
    
### Program:
```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Player_movement : MonoBehaviour
{
    // Start is called before the first frame update
    public float speed;
    void Start()
    {
        float xdir = Input.GetAxis("horizontal") * speed;
        float zdir = Input.GetAxis("vertical") * speed;
        transform.position=new Vector3(xdir,zdir);
    }

    // Update is called once per frame
    void Update()
    {
        
    }
}

```
### Output:


![Screenshot 2025-03-19 152433](https://github.com/user-attachments/assets/f5c1d1e7-ee36-48a5-a4a7-ba7067996cb2)
![Screenshot 2025-03-19 152511](https://github.com/user-attachments/assets/288917fa-47f1-48a7-946a-84618c981368)







### Result:
Thus the simple movement behavior was implemented successfully.
