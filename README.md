### Overview

The build step invokes the TypeScript compiler to create ES5 javascript
files and source maps from the `.ts` files. Run with:

    To install `npm install`

    To build: `npm run tsc`

    To build and run `npm run tsc-and-serve`

    To build and test `npm run tsc-and-test`

### Issue

Tests run successfully with this initial setup.
 
... But as soon as the 'test' files are moved 
from the src/test folder into the src folder ( along with some minor transforms to work
in the new location) then the tests fail with an obscure error message.
  
To repro this 

  - 1) rename the 'src' folder to 'src-good'

  - 2) rename the 'src-bad' folder to 'src'  

  - 3) rerun the tests. 