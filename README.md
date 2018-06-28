# jquery-accordion-plugin
In this project i have created a basic jquery pluginn with customization can be provided by users for creating a best accordiion on thier website with basic knowledge
 To created accordion in your webpage just follows these steps
 1.Create an container for placing your accordion.(if possible Give it a class of '.accordion' and use div as a container)
 2.For all of heading create a conatiner with class '.accordion-control'
 3. For contents of each contaainer create container with class '.accordion-panel'
 4. select your accordion container using jquery and use $().accordion() method
 ex
      <div class="accordion">
            <button class="accordion-control" >header 1</button>
            <div class="accordion-panel">
                content 1
            </div>    
        </div>
         <script> 
            $('.accordion').accordion(options);
           </script>
           
           
  Note: you can custom control your style and property by passing an object in your accordion() function.
  To control style
  use Ex:
   <script> 
            var options={
                accordionCss:{
                    width:"60%",
                    margin:"1em auto 1em auto",
                },
                speed:300
            };
            $('.accordion').accordion(options);
            </script>
            Also For controlling style of outer Box use accordionCss as inner object and pass jquery Style
            For controlling style of control Element use controlCss as inner object and pass jquery Style
            For controlling style of Panel Element use panelCss as inner object and pass jquery Style
