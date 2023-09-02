# 3D Modeling
---
1. Keep vertices aligned on the voxel grid while maintaining one pixel per 0.063 meters. (Each locked unit in Blender represents one pixel long)
2. Stray from using “voxel” looking structures and props, don’t refrain from creating interesting shapes and angles.
3. Keep models relative to the size of the player capsule.
4. Unwrap based on Cube Projection, might require tweaking for more complex/higher polygon count objects.


Pixel Perfect Modeling Example [Video](https://www.youtube.com/watch?app=desktop&v=RQVAUaSUP-k)

# Scripting
---
The general workflow for scripting should uphold best practices that will make code more easily readable, well-structured, and maintainable.
#### What should a script be?

When writing a script, we must have a clear goal in mind. Generally, larger problems can be broken down into smaller problems, which we can organize as functions in a script. A script should generally focus on handling the functionality for just one aspect of the game, for example moving the character, or lerping an object's position.
#### Proactively documenting code functionality

To make code more readable, and easier to maintain, we should write docstrings. Docstrings will enforce that we label each function with a description, a list of arguments and anything we should know about them, and what the function returns, along with anything we should know about that.

In addition, adding in-line comments, to help guide the person trying to read the code can provide more granular context than function level descriptions with docstrings. 

#### Scripting Workflow

1. In Plastic, if you are on main, ensure you have pulled the most up-to-date version. If you're on a branch and doing work in part of the project that could've been largely organizationally modified by someone else, then consider merging main into your branch before continuing working (you will likely be required to resolve conflicts at this point). Otherwise, continue working on the branch.
2. Identify the functionality you want to implement, or the problem you want to address with a script. The script should address one particular piece of functionality at the lowest level. At higher levels, scripts that help organize/control the flow of the game may also exist.
3. Segment sections of that problem into "smaller things that need to happen" in order to solve the issue. These will be your functions.
4. Write your function boilerplate (set up the function names, function types, parameters, return types, etc).
5. Go through the functions you have boilerplated and ensure each one has a docstring (see below for docstring example).
```c#
void RotateBackpack(Transform initTransform)
	//Rotates the object this script is placed on based on mouse movement and 
	//an initial Transform. Also note, the up and right of the object in Unity
	//must actually be aligned with the object's "front".
	//
	//Args:
	//    Transform initTransform - The transform to use for rotating around.
	//Returns:
	//    void
    {
        float mouseXDelta = Input.GetAxis("Mouse X");
        float mouseYDelta = Input.GetAxis("Mouse Y");

        transform.Rotate(initTransform.up, mouseXDelta);
        transform.Rotate(initTransform.right, mouseYDelta);
    }
```
6. Incrementally test functionality when you believe a feature that you can test is in a testable state. 
7. Commit to your branch in small increments, when you make valuable progress.
8. When you complete your work, ensure that it works properly, and that it is cleanly segmented and structured. At this point, you should push all you work, switch to main, and merge your work back into main.
# Shaders
---


# Particles
---

