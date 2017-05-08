
  ------------
  Refferences
  ------------

    1. BEM - Block - Element - Modifier
    ------------------------------------------------------------------
      BEM is a naming convention for css and is a good way to keep css
      clean, readible and reusable. 
      
      http://getbem.com/
    ------------------------------------------------------------------

    2. ITCSS - Inverted Triangle CSS
    ------------------------------------------------------------------
      ITCSS is css architecture the idea is to overcome the typical 
      issues assoiated with css, including specificity, repetitive
      css and css structure.
      
      Specificity Cone
      ----------------
        The idea here is that with are order are CSS by specificity,
        and as you can see with this simple cone that area inbetween
        settings is the largest that means is is the least specific.

        Settings      ----                      ---- Site Vars and sttings
        Tools         ------                  ------ Mixins and functions
        Generic       --------              -------- Reset etc
        Base          ----------          ---------- html, inputs ,tables etc
        Objects       ------------      ------------ Container, rows etc
        Components    --------------  -------------- Home search, product item. etc
        Overrides     ------------------------------ !importants and high specificity
      
      http://itcss.io/
      https://csswizardry.com/
      http://goo.gl/HLDU0U
    ------------------------------------------------------------------

    3. OOCSS - Oject Oriented CSS
    ------------------------------------------------------------------
      OOCSS is a methodology,a way of thinking about CSS. The idea
      being to write css to be more resuable, scalable and 
      maintainable.    
      
      https://appendto.com/2014/04/oocss/
    ------------------------------------------------------------------

    4. CSS Namespacing
    ------------------------------------------------------------------
      CSS namespacing is not original and the way I use it is
      similar to the great Harry Roberts of CSS wizardry. The idea 
      being you can quickly and easily tell what type of
      item a class is. It could be an object, a component or a helper.
      From this you are able to determine if changing the CSS on this
      class should effect other parts of the code.  
      
      https://goo.gl/5L3BxV
    ------------------------------------------------------------------

    5. Flex
    ------------------------------------------------------------------
      Flex is a great way to center, align and order items on our
      page, that would otherwise be alot more difficult to achive.
      It is important to note that you should use a fallback for
      non supported browser versions.  
      
      https://goo.gl/WySM2z
    ------------------------------------------------------------------



  -----------
  Namespacing
  -----------

    1. Objects - Sits within the objects folder: o-
    ------------------------------------------------------------------
      Objects are simply elemnts that have  none spefic on blocks 
      that make up the page. An example of a object would would be
      a container, it is used in muitple places but does not effect
      one spefic block on the page unlike styling for a carousel 
      for exmaple.

      Altering these objects when maintaining the code will effects
      many instances so it is not recommended.  
    ------------------------------------------------------------------

    2. Components - Sits within the components folder: c-
    ------------------------------------------------------------------
      Components are what combine with objects to style our page
      they are the spefic styles to out page elements sich as a 
      carousel block.

      A good example would be a contact form, the inputs of the form
      will have some base styling from the generic syling set across
      all inputs but the spefic layout of a certain form is achived
      by the component.
    ------------------------------------------------------------------

    3. Utilities - Sits within the utilities folder: u-
    ------------------------------------------------------------------
      Utilities are normally actions such as clearfixes and hidding
      elements.
    ------------------------------------------------------------------

    4. States - Sits within individual components: is- / has-
    ------------------------------------------------------------------
      States or self explanatory, they are for items such as a
      accordion. An accordion has two states the default which is
      closed and then a open sate to style this open state we 
      would use an class of is-open for example. 
    ------------------------------------------------------------------

    6. JS Calls - Classes added to HTMl: js-
    ------------------------------------------------------------------
      JS calls are simply classes given to elements which are then 
      selected with JS.
    ------------------------------------------------------------------

    7. Grid - Sits within individual components: g-
    ------------------------------------------------------------------
      The grid namespace is used to controll the grid layout on the
      site. There is more documentation below on using the grid.
    ------------------------------------------------------------------



  ----
  Grid
  ----

    Firstly the inbuilt grid can be disabled in the settings, however
    it goes hand in hadn with the rest of the framework and has been 
    built to work with it. 

    The way in which the frid is called is simple, it is class based,
    so for example lets say I want a grid with 2 items in it (50% with gutter)
    I would add the class g-{Screen Size}-2. The last number indicates the 
    amount of items within the grid. The middle poperty is the device
    size which you would like the grid to be for,
    So an exmaple would be g-mob-2, this means on mobile there will
    be two items in the row.
    
    See more inside of tools/grid.scss