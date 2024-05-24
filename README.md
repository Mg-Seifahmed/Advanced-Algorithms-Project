# Advanced-Algorithms-Project


 # 2D Closest Pair Problem Using Divide and Conquer Approach

The 2D closest pair problem involves finding the pair of points in a set that are closest to each other. This problem can be efficiently solved using the divide-and-conquer approach, which has a time complexity of O(n log n).



1. **Sort the Points**:
   - Sort the points based on their x-coordinates. Let's call this sorted array `Px`.
   - Sort the points based on their y-coordinates. Let's call this sorted array `Py`.

2. **Divide**:
   - Find the median point in the sorted array `Px` to divide the points into two equal halves. Let this median point be `mid_point`.
   - The dividing line is a vertical line passing through `mid_point`.

3. **Conquer**:
   - Recursively find the closest pair of points in the left half and the closest pair of points in the right half.
   - Let the minimum distance found in the left and right halves be `delta`.

4. **Combine**:
   - Consider a strip of width `2 * delta` centered at the dividing line.
   - Create an array `Sy` containing points within this strip, sorted by their y-coordinates.
   - For each point in `Sy`, check distances only with the next 7 points (due to geometric properties, it's sufficient to check only the next 7 points).
   - Update the minimum distance if a closer pair is found in this strip.

5. **Return the Result**:
   - The smallest distance found in the above steps is the distance between the closest pair of points.

This approach ensures that the problem size is reduced in each recursive step, leading to an overall efficient algorithm.

# refrences 
link: https://youtu.be/6u_hWxbOc7E?si=yu2touSBD2omr-Ub
GeekForGeeks: https://youtu.be/9mZ9CY2oOIE
# project video 
**link** : https://youtu.be/9mZ9CY2oOIE

