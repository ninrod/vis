Dr. Chip's Visual Block Commands
=========

* This is a mirror of the vim script available at [drchip's website](http://www.drchip.org/astronaut/vim/vbafiles/vis.vba.gz)

Current Version: 
--------------
* version: `21e`, as of `10.fev.2016`

----------------
Visual Commands:
----------------
    B

    Use V, v, or ctrl-v to visually mark some region.  Then use
       :B cmd     (this command will appear as:   :'<,'>B cmd)

    The command will then be applied to just the visually selected region.
    For examples:

      Use ctrl-v to select a column and then do a substitute on just that column.
      ctrl-v ..move.. :B s/pattern/becomes/

      Use ctrl-v to select a column, then apply an external filter to just that column.
      ctrl-v ..move.. :B !sort


----------------
Visual Searches:
----------------

    S

    Use V, v, or ctrl-v to visually mark some region.  Then use
        :S pattern   (this search will appear as     :'<,'>S pattern)

    The search will then be applied to just the visually selected region.
    It may be repeated with n and N commands, too (without having to
    re-mark the region).  A plain S will apply the last :S-pattern
    to the latest selected region.


-----------------
Related Subjects:
-----------------

 * For incrementing/decrementing numbers, dates, and letters in a column: see vimscript#670 and vimtip#150
 * For sorting based on a column (column-restricted, whole lines but column-keyed), see vimtip#588
 * For overwriting visual blocks with other visual blocks: see vimtip#808
 * For more on applying substitutes to a visual block: see vimtip#63
 * For swapping pairs of visual blocks: see vimtip#329
