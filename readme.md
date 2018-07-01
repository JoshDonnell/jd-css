--------------------
  JD Sass Framwork
--------------------
  

  ------------
  Introduction
  ------------

This is a lightweight SASS framework, following multiple methodologies
including BEM, ITCSS, OOCSS, CSS Namespacing and also flex.



  ----------
  References
  ----------

    1. BEM - Block - Element - Modifier
    ------------------------------------------------------------------
      BEM is a naming convention for CSS and is a good way to keep CSS
      clean, readable and reusable.
      
      http://getbem.com/
    ------------------------------------------------------------------

    2. ITCSS - Inverted Triangle CSS
    ------------------------------------------------------------------
      ITCSS is CSS architecture the idea is to overcome the typical 
      issues associated with CSS, including specificity, repetitive
      CSS and CSS structure.
      
      Specificity Cone
      ----------------
        The idea here is that we would order the CSS by specificity,
        this is illustrated with the simple cone, the area in between
        settings is by far the largest that means is the least specific. 
        Whereas the area between the Overrides is tiny meaning they have
        a high specificity.
      
      http://itcss.io/
      https://csswizardry.com/
      http://goo.gl/HLDU0U
    ------------------------------------------------------------------

    3. OOCSS - Oject Oriented CSS
    ------------------------------------------------------------------
      OOCSS is a methodology, a way of thinking about CSS. The idea
      being to write CSS to be more reusable, scalable and 
      maintainable. 
      
      https://appendto.com/2014/04/oocss/
    ------------------------------------------------------------------

    4. CSS Namespacing
    ------------------------------------------------------------------
      CSS namespacing is not original and the way I use it is
      similar to the great Harry Roberts of CSS wizardry. 
      The idea being you can quickly and easily tell what type
      of item a class is. It could be an object, a component 
      or a helper. From this you are able to determine if 
      changing the CSS on this class should effect other 
      parts of the code.  
      
      https://goo.gl/5L3BxV
    ------------------------------------------------------------------


    
  -----------
  Namespacing
  -----------

    1. Objects - Sit within the objects folder: o-
    ------------------------------------------------------------------
      Objects are simply elements that have  none specific on blocks 
      that make up the page. An example of an object would-would be
      a container, it is used in multiple places but does not effect
      one specific block on the page unlike styling for a carousel 
      for example.

      Altering these objects when maintaining the code will effects
      many instances so it is not recommended.  
    ------------------------------------------------------------------

    2. Components - Sit within the components folder: c-
    ------------------------------------------------------------------
      Components are what combine with objects to style our page
      they are the spefic styles to out page elements sich as a 
      carousel block.

      A good example would be a contact form, the inputs of the form
      will have some base styling from the generic syling set across
      all inputs but the spefic layout of a certain form is achived
      by the component.
    ------------------------------------------------------------------

    3. Utilities - Sit within the utilities folder: u-
    ------------------------------------------------------------------
      Utilities are normal actions such as clearfixes and hiding
      elements.
    ------------------------------------------------------------------

    4. States - Sit within individual components: is- / has-
    ------------------------------------------------------------------
      States or self-explanatory, they are for items such as a
      accordion. An accordion has two states the default which is 
      closed and then an open state to style this open state we 
      would use a class of is-open for example. 
    ------------------------------------------------------------------

    6. JS Calls - Classes added to HTMl: js-
    ------------------------------------------------------------------
      JS calls are simply classes given to elements which are then 
      selected with JS.
    ------------------------------------------------------------------
