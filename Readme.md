npm i -D parcel

<!-- 
running that command will create 3 things:

node_modules: a directory containing all the packages we install from npm but also, those packages’ dependencies. Say you need package A but it requires package B, well, you could find both in here. Currently, everything you find inside this directory, is required in one way or another by Parcel! 
⚠️We will avoid pushing this directory to GitHub because it can get heeeeavy ⚠️

package.json : This file contains a single JSON structure with different keys that will help us describe our project. From adding keys for the author , license and description of our project, to describing the dependencies of our project! Right now, the document only has a devDependencies listing Parcel with a number, this number is the current version our project is using, this is important for maintenance and support in the future.

package-lock.json : This file, similar to the previous one in many ways, contains the full dependency map. Package A needs package B and C and package X needs B ? Well, a map of what needs what is here! This will help us avoid installing packages if we already have them! -->


<!-- Using the Tailwind imported module in styles.css we use: -->

<!-- npx parcel index.html -->

<!-- Final changes with npm/leaflet, run command: -->

npm run build

<!-- output:
> build
> parcel build

✨ Built in 495ms

dist/index.html                       465 B     51ms
dist/my-parcel-app.a017c8ff.css     4.61 kB     58ms
dist/my-parcel-app.99cdbd0f.js     149.4 kB    133ms
dist/my-parcel-app.9b42016c.css    10.53 kB     67ms
dist/layers.760a0456.png              696 B     38ms
dist/layers-2x.b7b89169.png         1.26 kB     24ms
dist/marker-icon.3f7d3721.png       1.47 kB     47ms -->

<!-- output directory 'dist' contains machine optimized code; no spaces or lines which humans require reading! -->



<!-- Close whatever files you opened, run -->
npm run build
<!-- again and then run (the x here stands for executable) -->
npx serve dist

<!-- runs local webserver: -->
http://localhost:3000