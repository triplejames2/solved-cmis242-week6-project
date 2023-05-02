Download Link: https://assignmentchef.com/product/solved-cmis242-week6-project
<br>
The third programming project involves writing a program that draws two types of shapes, ovals and rectangles. This program consists of six classes. The first class is the <sub>Shape</sub> class, which is an abstract class that extends the predefined Java class <sub>Rectangle</sub>. It should contain two instance variables, the color of the shape and whether the shape is solid or hollow. It should also contain a class (static) variable that keeps track of how many shapes have been created.. It should have three instance methods, one class method and one abstract method:

<ol>

 <li>A constructor that accepts three parameters for the purpose of initializing the characteristics of the shape, a <sub>Rectangle</sub> object that defines the dimensions and position of the shape, the color of the shape and whether the shape is solid or hollow. It should also update the number of shapes created so far.</li>

 <li>An instance method named <sub>setColor</sub> that accepts the <sub>Graphics</sub> object as a parameter and sets the color for the next draw operation to the color of the current shape.</li>

 <li>An instance method named <sub>getSolid</sub> that returns whether the shape is solid or hollow.</li>

 <li>A class method named <sub>getNoOfShapes</sub> that returns the number of shapes created so far.</li>

 <li>An abstract method named draw that accepts a <sub>Graphics</sub> object as a parameter.</li>

</ol>

The <sub>Shape</sub> class has two subclasses. The first is <sub>Oval</sub>. It should have the following two methods:

<ol>

 <li>A constructor that accepts three parameters for the purpose of initializing the characteristics of the shape, a <sub>Rectangle</sub> object that defines the dimensions and position of the shape, the color of the shape and whether the shape is solid or hollow.</li>

 <li>An overridden method <sub>draw</sub> that draws the <sub>Oval</sub> object on the <sub>Graphics</sub> object passed as a parameter.</li>

</ol>

The second subclass is <sub>Rectangular</sub>. It should have the following two methods:

<ol>

 <li>A constructor that accepts three parameters for the purpose of initializing the characteristics of the shape, a <sub>Rectangle</sub> object that defines the dimensions and position of the shape, the color of the shape and whether the shape is solid or hollow.</li>

 <li>An overridden method <sub>draw</sub> that draws the <sub>Rectangular</sub> object on the <sub>Graphics</sub> object passed as a parameter.</li>

</ol>

The fourth class is named <sub>Drawing</sub>, which should extend the predefined Java class <sub>JPanel</sub>. It has one instance variable that contains the shape that is currently drawn.. It should have three methods:

<ol>

 <li>An overridden <sub>paintComponent</sub> method that draws the current shape on the <sub>Graphics</sub> object that is passed to it as a parameter. It should also draw the number of shapes that have been created thus far in the upper left corner.</li>

 <li>An overridden <sub>getPreferredSize</sub> method that specifies the dimensions of the drawing panel as 200 pixels wide and 200 pixels high.</li>

 <li>An instance method named <sub>drawShape</sub> that is passed the current shape to be drawn. It first checks whether the shape provided will completely fit within the panel. If not, it throws an <sub>OutsideBounds</sub> Otherwise, it saves the shape in the corresponding instance variable. It then calls repaint to cause that shape to be drawn.</li>

</ol>

No additional public methods should be included in any of the above classes.

The fifth class named <sub>OutsideBounds</sub> should define a checked exception.

The sixth class named <sub>Project3</sub> should contain the main method. It should generate the GUI shown below:







The combo-box for the shape type should allow two choices, either <em>Rectangle</em> or <em>Oval</em>. The combo-box for the fill type should also allow two choices, either <em>Hollow</em> or <em>Solid</em>. The combobox for the color should allow seven choices, <em>Black</em>, <em>Red</em>, <em>Orange</em>, <em>Yellow</em>, <em>Green</em>, <em>Blue</em> or <em>Magenta</em>.

Clicking the <em>Draw</em> button should first check whether any non integer values have been entered in

any of the fields that require integers. If so, an error message should be displayed in a JOptionPane window. Otherwise an appropriate <sub>Shape</sub> object should be created and passed to the <sub>drawShape</sub> method of the <sub>Drawing</sub> class. If that call results in an <sub>OutsideBounds</sub> exception being thrown, an appropriate error message should be displayed in a <sub>JOptionPane</sub> window.

Be sure to follow good programming style, which means making all instance variables private, naming all constants and avoiding the duplication of code. Furthermore you must select enough different kinds of shapes to completely test the program.