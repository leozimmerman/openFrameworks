## Adding ofxSyphon to Xcode:
	OF Plugin -> add ofxSyphon
	Framework Search Path : ../../../addons/ofxSyphon/libs/Syphon/lib/osx
	Header Search Path: -Check from ofxSyphon example project

## Adding ofxOsc to Xcode:
	OF Plugin -> add ofxOsc
	Header Search Path: -Check from OF_ROOT/examples/addons/oscReceiver	


## Running OF 0.8.0 Projects in OS X 10.10
	
	- error: There is no SDK with the name or path '/Users/leo/Development/of_v0.8.0_osx_release/libs/openFrameworksCompiled/project/osx/macosx10.9' :
	
	In XcodeProject Navigator search for openFremeworks project->Build Settings-> Base SDK

	- error:’openssl/opensslconf.h' file not found: 
 	in CoreOF.xcconfig:
	HEADER_OPENSSL = "$(OF_PATH)/libs/openssl/include"
	OF_CORE_HEADERS +=  $(HEADER_OPENSSL)

	- error: "_FreeImage_Initialise", referenced from:
	in CoreOF.xcconfig:
	OF_CORE_LIBS += $(LIB_FREEIMAGE)

	- error: "_FT_Done_FreeType", referenced from:
	in CoreOF.xcconfig:
	OF_CORE_LIBS += $(LIB_FREETYPE)
	
