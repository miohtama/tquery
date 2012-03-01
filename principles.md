* to go in core, you need to be used everytime!
* tQuery is only an API change, no change in semantic
  * other functions
  * other default
  * same semantic
* a good api is
  * clear (clear for whom ?)
  * stable
  * well documented
* you must be able to easily go back and forth between three.js and tQuery.
* core has no require.js
  * dependancy between plugins handled by require.js
* tquery.js core depends only on the three.js
* the only global defined is tQuery
* not to disrupt devs habits is important for a lib
* put sanity check when possible
  * any misuse should be detected as soon as possible
* instrumentability
  * stuff must be usable by computers
* between 2 alternatives, one cooked, one raw, pick the raw one
  * especially in case of doubt

## directions
* "For those who want to know webgl, good news! You already know it, just replace j by t!"
  * make this statement true
* "webgl should not be harder than playing with lego."

## Name Conventions
* suppose you want to create a material plugin about fireball
* file tquery.fireballmaterial.js
* classname tQuery.FileballMaterial
* ctor: tQuery.FileballMaterial and new tQuery.FileballMaterial()
* naming convention is more readable

* provide .create*() functions to avoid new everywhere
  * see in Object.Create()
  * seen in domElement.createElement()

* geometry varname represents tQuery.Geometry instance
  * tGeometry varname represents THREE.Geometry
  * and so on in the principles
