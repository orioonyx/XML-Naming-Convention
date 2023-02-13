# XML-Naming-Convention
![](https://user-images.githubusercontent.com/74607521/218515659-9c9fecb9-1d89-4486-8062-14bfa0566a8b.png)

Android uses XML to define the layout of its user interface elements. The structure and naming of XML elements are important in ensuring that the user interface is well-defined, easy to understand, and maintainable.

Here are some general naming conventions for Android XML files:
<br/><br/>

# Basic Principle
    <WHAT>-<WHERE>-<DESCRIPTION>-<SIZE>


`WHAT`
------------------------------------

Indicate what the resource actually represents, often a standard Android view class. Limited options per resource type.

ex) activity, fragment, view, item, layout...

`WHERE`
------------------------------------

Describe where it logically belongs in the app. Resources used in multiple screens use all, all others use the custom part of the Android view subclass they are in.

ex) all, main, home, login, user...

`DESCRIPTION`
------------------------------------

Differentiate multiple elements in one screen.

ex) title, content, info, profile...

`SIZE` (optional)
------------------------------------

Either a precise size or size bucket. Optionally used for drawables and dimensions.

ex) 24dp, small...
<br/><br/><br/>

# Layouts

    <WHAT>_<WHERE>_<DESCRIPTION>.xml

ex) activity_main.xml, fragment_onboarding, item_product, fragment_product_search
<br/><br/>

# Strings

    <WHERE>_<DESCRIPTION> or all_<DESCRIPTION>

ex) main_title, user_namehint, login_titlehint, all_done, all_fail
<br/><br/>

# Drawables

    <WHAT>_<WHERE>_<DESCRIPTION>_<SUFFIX>
    
    <SUFFIX> : <DIRECTION>_<SHAPE>_<OUTLINE>_<STATE>_<COLOR>_<SIZE>
  
`WHAT` : ic, bg, img, logo...<br/>
`WHERE` : navi, tab, home, login...<br/>
`DESCRIPTION` : check, like, btn, close...<br/>
<br/>

`SUFFIX` :

**DIRECTION** : left, right, up, down...<br/>
**SHAPE** : circle, square, roundsquare...<br/>
**OUTLINE** : outline, border...<br/>
**STATE** : on, off, activated, disabled, normal...<br/>
**COLOR** : white, black...<br/>
**SIZE** : 24dp, small...

ex) ic_login_btn_disabled.png, ic_heart_on.png, ic_check_white_small.png
<br/><br/>

# IDs

    <KIND>_<WHERE>
    
`KIND` :

(most commonly used android view classes)
    
| View Class        | Abbrevation       |
| ----------------- | ----------------- |    
| CoordinatorLayout | cdl               |
| ConstraintLayout  | csl               |
| LinearLayout      | ll                |
| RelativeLayout    | rl                |
| AppBarLayout      | abl               |
| Button            | btn               |
| EditText          | et                |
| TextView          | tv                |
| ProgressBar       | pb                |
| Checkbox          | chk               |
| RadioButton       | rb                |
| ToggleButton      | tb                |
| Spinner           | spn               |
| Menu              | mnu               |
| ListView          | lv                |
| RecyclerView      | rv                |
| GalleryView       | gv                |


ex) iv_profile, et_login_username, btn_submit, rv_product
<br/><br/>

# Dimensions

    <WHAT>_<WHERE>_<DESCRIPTION>_<SIZE>

`WHAT` :

| Prefix    | Usage       |
| --------- | ----------- |
| width     | width in dp |      
| height    | height in dp |  
| size      | if width == height |  
| margin    | margin in dp |          
| padding   | padding in dp |          
| elevation | elevation in dp |  
| keyline   | absolute keyline measured from view edge in dp |          
| textsize  | size of text in sp |  
        
ex) height_toolbar, textsize_nomal
<br/><br/>

