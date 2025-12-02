npm i -D parcel

<!-- 
running that command will create 3 things:

node_modules: a directory containing all the packages we install from npm but also, those packages’ dependencies. Say you need package A but it requires package B, well, you could find both in here. Currently, everything you find inside this directory, is required in one way or another by Parcel! 
⚠️We will avoid pushing this directory to GitHub because it can get heeeeavy ⚠️

package.json : This file contains a single JSON structure with different keys that will help us describe our project. From adding keys for the author , license and description of our project, to describing the dependencies of our project! Right now, the document only has a devDependencies listing Parcel with a number, this number is the current version our project is using, this is important for maintenance and support in the future.

package-lock.json : This file, similar to the previous one in many ways, contains the full dependency map. Package A needs package B and C and package X needs B ? Well, a map of what needs what is here! This will help us avoid installing packages if we already have them! -->


