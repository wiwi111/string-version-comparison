# string-version-comparison
Util file with methods for getting text with differences from changing old to new version of given text.
Comparing old and new versions of String. Result is a string with highlighted by tag words which have changed.
Methods:
* **getComparisonString(String oldInstance, String newInstance)** : 
   Returns result string which combines old value with highlighted added and deleted words.
	  * Added words are between [\<added\>] and [\</added\>].
	  * Deleted words are between [\<deleted\>] and [\</deleted\>].
         
    Example:
    
    newInstance= "Chcecie bajki. Byla sobie pchla szachrajka";    
    oldInstance= "Chcecie bajki oto bajka. Byla sobie pchla szachrajka";    
    result = "Chcecie [\<added\>]bajki. [\</added\>][\<deleted\>]bajki oto bajka. [\</deleted\>]Byla sobie pchla szachrajka ";

* **getComparisonStringHtmlDecoratedWithClasses(String oldInstance, String newInstance)** :
	 Returns result string which combines old value with highlighted added and deleted words.
	   * Added words are between \<span class=\"addedWords\"\> and \</span\>.
	   * Deleted words are between \<span class=\"deletedWords\"\> and \</span\>.
  
