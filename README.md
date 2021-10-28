# menuLevelSwipe
 levels sorted horizontally with possibility to swipe between each one.

OG By "Akbar Project" : https://www.youtube.com/watch?v=GURPmGoAOoM

1. New Scene.
2. Make a new canvas:
    - Render mode = World Space
    - refer your Event Camera
3. Make a new Scrollview : 
    - Width: 650
    - Height: 367
    - Scroll Rect Component/Vertical : Uncheck
4. Image/Color : white
5. Delete "Scrollbar Vertical" from the Scroll View object in the hierarchy. You must now have a Scroll View with as childs, Viewport and Scrollbar Horizontal.
6. Scrollbar Horizontal/Rect Transform/Height = 0
7. Resize Viewport to the canvas size
8. Viewport/Content/New TMP_Button
    - Width: 160
    - Height: 240
9. Viewport/Content/TMP_Button/Text : Rename to "Level (1)" (unity will autonamitcally increment numbers on duplication), set as text "level 1", customize font size and stuff
10. Viewport/Content : Add Component : Content Size Fitter
11. Horizontal Fit : preferred size
12. Viewport/Content : Add Component : Horizontal Layout Group
    - Child alignement : Middle left
    - Padding : 
        - Left: 255
        - Right : 255
        - Spacing : 40
13. Test. The scrolling should be working fine.
14. New Script : swipeMenu
15. Attach it to "Content"
16. refer "Scrollbar Horizontal" to "Scrollbar" field.