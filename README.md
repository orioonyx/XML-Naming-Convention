# XML-Naming-Convention
___

A successful XML naming convention should adhere to the following guidelines:

### Basic Principle
    <WHAT>-<WHERE>-<DESCRIPTION>-<SIZE>
    
<br/>
#### <WHAT>

Indicate what the resource actually represents, often a standard Android view class. Limited options per resource type.

ex) activity, fragment, view, item, layout...


#### <WHERE>

Describe where it logically belongs in the app. Resources used in multiple screens use all, all others use the custom part of the Android view subclass they are in.

ex) all, main, user...


#### <DESCRIPTION>

Differentiate multiple elements in one screen.

ex) title, content, info, profile...


#### <SIZE> (optional)

Either a precise size or size bucket. Optionally used for drawables and dimensions.

ex) 24dp, small...
