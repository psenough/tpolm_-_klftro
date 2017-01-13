Jetski

possible Demobit 2017 64k attempt?!

to convert AHX file into url-encoded string you use Gasman's binhexjs.rb to create a .js file and then copy paste it into the source code
you'll need to install ruby first,
on windows use ruby installer for ruby 2.3.3
http://railsinstaller.org/en

then you'll be able to run 
`ruby binhexjs.rb THX.syphus-Jetski[Twin_Beam_cover].ahx >> AHXdump.js`
or simply call `binhexjs.bat`

test stuff launching index.html

to compile the javascript with closure compiler you should write this on the console

`java -jar compiler.jar --compilation_level ADVANCED_OPTIMIZATIONS --js jetski.js --externs closure_audiocontext.js --externs closure_ctxhash.js --js_output_file=jetski_closure.js`

to convert it to .png self extractable you should write this on the console

`ruby pnginator.rb parsley_closure.js tpolm_-_parsley_state.png.html`
