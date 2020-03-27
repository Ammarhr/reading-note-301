# Read-01:

## Responsive Web Design:

**What is Responsive  Web Design?**
**Responsive web design** is the practice of how to  build a website that can be suitable to work on every device and every screen size in order to provide a gratifying experience for everyone. to make desktop computer and cell phone users to benefit from responsive websites alike all.

**ًwhat the difference between Responsive vs. Adaptive vs. Mobile?**
**Responsive:** 
- means to react quickly and positively to any change.
- responsive websites continually and fluidly change based on different factors, such as viewport width.
- responsive has the benefits of being all three, responsive, adaptive, and mobile.
**Adaptive:**
- means to be easily modified for a new purpose or situation.
- adaptive websites are built to a group of preset factors
**Mobile:**
- means to build a separate website commonly on a new domain solely for mobile users.


#### Responsive web design is broken down into three main components:
1.  **Flexible Layouts:** is the practice of how to  build the layout of a website with a flexible grid. capable of dynamically resizing to any width. these flexible grids are built using relative length units (% or em for  width, margin.. etc).
2. **Media queries:** is an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances.
we can use **Media queries** by two ways:
- sing the ``@media`` rule inside of an existing style sheet, importing a new style sheet using the ``@import`` rule
- linking to a separate style sheet from within the HTML document.
>>is recommended to use the ``@media`` rule inside of an existing style sheet to avoid any additional HTTP requests.
>>

we can use Logical operators in media queries,it's help build powerful expressions. the operators that we can use are: "and", "not", and "only".
3. **Flexible media:** . As viewports begin to change size media doesn’t always follow suit. Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

----------------------------------------------------------------

## What is "Float":
**Float** is a positioning property in **CSS**.  that make the images set into the page such that text wraps around them as needed. using ``float-left`` & ``float-right`` we can controll the position of the image based on the element arround (for EX: the box of text).

### What are floats used for?
In additon of the simple example of wrapping text around images, floats can be used to create entire web layouts.
It also helpful  for layout in smaller instance.

### Clear porperty:
 ``Float``'s sister property is ``clear``. An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float.

 ### Problem with Floats and how to fix it:
 1. **Pushdown** is a symptom of an element inside a floated item being wider than the float itself . Most browsers will render the image outside the float
  >> Quick fix: Make sure you don't have any images that do this, use overflow: hidden to cut off excess.
  >>
2. **Double Margin Bug** - Another thing to remember when dealing with IE 6 is that if you apply a margin in the same direction as the float, it will double the margin. 
>> Quick fix: set display: inline on the float, and don't worry it will remain a block-level element.
>>
3. The **3px Jo**g is when text that is up next to a floated element is mysteriously kicked away by 3px like a weird forcefield around the float.
>> Quick fix: set a width or height on the affected text.
>>
4. In **IE 7** , the Bottom Margin Bug is when if a floated parent has floated children inside it, bottom margin on those children is ignored by the parent.
>> Quick fix: using bottom padding on the parent instead.
>>