* Tab separated
* Pound (#) sign starts new section
  * Propsition-dict
    1. Proposition ID (some unique number)
    2. Alias of the proposition (in an automatic system, this can be the first mention).
    3. List of mentions / IMPLICIT (arbitrary length) 
    4. More mentions ...
  * #entities
    0. **NOTE**: consider adding unique id (similarly to propositions).
    1. Alias (unique)
    2. Mentions:
       * Each composed of:
         * string (without tabs and brackets).
         * number of occurences in square brackets, right after the mention.
       * Semi colon
       * Entailments (**TODO**)
  * #proposition:
    * For each proposition in the proposition dict:
      * In the line with #proposition - proposition ID ; time-stamp (of first tweet with mention of the propsition) [TAB delimited]
      * #predicates - list of templates
        * each template - words and argument-links  [number of proposition-mentions and ID of source tweets] ; ENTAILMENT
      * arguments - list of arguments, each with:
        * argument-ID  TAB label  TAB  alias\id-of-entity\prop [number of argument-mentions and ID of source tweets]  
        
