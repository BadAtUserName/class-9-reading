# class-9-reading
reading notes from class 9.

q. Why are forms so important in web development?<br>
a. They give the user a way to interact with the page, and the developer/page a way to <br>collect data that may be used later.<br>
q. When designing a form, what are some key things to keep in mind when it comes to user experience?<br>
a. Accessibility. To keep it easy for screen readers to use, if it sounds strange change it till it sounds better<br>
q. List 5 form elements and explain their importance.<br>
Form it defines the form, you cannot have a form without it.<br> 
Label which takes it’s value from the id it is associated with for form control, this is how you match them up.<br>
Input a single line text field<br>
Textarea a multiple line textfield<br>
Button gives dev and users a way to input data and track data and not give too many options. <br>

q. How would you describe events to a non-technical friend?<br>
a. Events are things you can interact with on a webpage that report things back to the code a developer wrote.<br>
q. When using the addEventListener() method, what 2 arguments will you need to provide?<br>
a. You need to add a type, a case sensitive strip that stands for the event type to listen for. The second thing needed is a listener, like click, submit or mousedown.<br>
q. Describe the event object. Why is the target within the event object useful? <br>
a. The argument of a handler function is an event object. The target recognizes the element that starts an event. <br>
q. What is the difference between event bubbling and event capturing?<br>
a. Events bubbling is how the browser handles events targeted at nested elements, Event <br>capturing means propagation of the event is done from ancestors grandparents, <br>parents to childern. Event bubbling is similar but done in the child element of the<br> DOM. Event capture first bubble later<br>



Forms and JS Events<br>	

Your First HTML Form<br>
First experience building web form<br>
What are webforms? <br> 
Main points of interaction betwixt user and website or app<br>
Allows user to enter data which is sent to web server 4 processing and storage<br> 
A web forms html is is made of up of or more form controls/widgets<br>
Controls can be sing or multi line feeds <br>
Drop down boxes<br>
Buttons<br> 
Checkboxes<br>
Radiobuttons<br>
     C. Designing your form<br>
	1. Take a step back and think about what you want to do<br>
	2. Keep it short and simple no one likes signing up for things<br>

   D. The < form > Element<br>
	1. All forms start with < form > <br>
		a. The element formally defines a form it’s an element container like section<br> 
		     or footer, but just for forms<br> 
	2. The action attribute defines the location URL where form data collected should<br>
	     be sent<br> 
	3. Method attri refs wh/ http meth send the data w. Usually get or post<br>
	4. Add the < from> into HTML BODY!!!!!!!!

  E. Label, input, textarea elements
	1. Contact form not complex the at a entry portion contains 3 text fields w. Label<br>
		a. Input field for name is single line text field<br>
		b. Input email input type of email<br>
		c. Input area for message is textearea a multiline text field.<br>
		d. Code example found at https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form
		e. The < li > elementstruct code to make styling easier. For usability include<br>
		     include explicit label for peace form control<br>
			1. Note the use of the for attribute on <label> which taks as it’s val<br>
			    id of form control w. Wh/ it is assoc. this is how to also a form<br>
			    control with it’s label<br>
		f. On input element the most important attribute is the type attribute.<br>
		   defines the way the input element appears and behaves. 
			1. In ex used the val text for 1st input, the default val for this attri<br>
			2. For 2nd input we use the val email. Refs single line text field that<br>
			    only access  a well formed email. 
			3. Turns text field intelligent preforms validation check<br>
			4. Note syntax of input vs. < textarea > </ textarea> oddity	 of HTML<br> 
			    input tag is void element does not need closing tag textarea is<br>
			    needs closing tag<br>
			5. To define input val do it up like a class<br>
			6. Textarea do it like a div<br>

  F. Button Element. 
	1. Need to submit form<br>
	2. Button element accepts 1 of 3 vals<br>
		a. Submit<br>
		b. Reset<br>
		c button<br>
	3. Click submit send forms data to webpage deed by action attri of form<br>
	4. Cling on reset button resets all the form widget to their default value immediately<br> 
		a. From ui view don’t do this it’s bad practice<br> 
		b. Click on button and does NOTHING!!!! Can def fuctiontwith js later.<br>

   G. Basic form styling<br> 
	1. Add style using < style > tag.<br> 
	2. Inside style use follow see link <br>
     
   H. Sending form data to your web server<br>
	1. Sending form data to server side can be tricky<br>
	2. Provide Name attribute for each form control names important on both sides<br>
	    client and severs sides. Tell browser which name to give each piece of data & on<br> 
	    server side they let the server handle each piece of data by name.<br>

III.  How to structure a web form<br>
     
  A. The flexibility of forms makes them a v complex structure in HTML<br>

  B. The < form > element. 
	1. Formally defines a form and attributes that set forms behavior<br>    
	2. FORBIDDEN TO NEST A FORM INSIDE ANOTHER FORM. CAN CAUSE REAL<BR>
	    FARKING PROBLEMS. 

  C. The < fieldset >	and < legend > element
	1. Fieldset es a way to create groups of widgets that share the same purpose for<br>
	    styling and semantic purpose<br>
	2. Can label by including a < legend > element just below the opening fieldset tag<br>
	3. Text connect in legend describes the purpose of the fieldset it is inside<br>
	4. See link for image<br>
	5. Screen readers will see ^ text as small juice, medium juice, large juice 1, 2, 3<br>
	6. Using above as example. When see radio buttons nest them inside of fieldset<br>
	    element<br> 
	7. Due to influence on assistive technology the fieldset element is one of the key<br>
	    elements for building accessible forms DO NOT ABUSE IT<br>
     
  D.  The < label > element<br>
	1. MOST IMPORTANT ELEMENT IF YOU WANT TO BUILD ACCESSIBLE FORMS<BR>
	2. Element is formal way to define a label for html form widget<br>
	3. w. Label assoc w. Input via for attr contains  input elements in id attri a screen<br>
	    readers will see “ name, edit text” <br> 
	4. Or can associate form control with label next form within label simplicity assoc it<br>
	5. Even in casses like this best practice to set for attribute to ensure assistive tech<br>
	    understand the relationship betwixt label and widget<br>
	6. Labels are clickable too<br>
		a. Advantage of properly set up labels is can click or tap label to active<br>
	                associated widget<br>
		b. Useful for controls like text inputs<br>
		c. V. Useful for radio buttons<br>
	7. Multiple labels<br> 
		a. Can put multiple labels on single widget but not a good idea as some<br> 
		    assistive tech can have trouble w. them<br>

