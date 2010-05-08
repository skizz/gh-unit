

default:
	xcodebuild -target "CombineLibs (3.0)" -configuration Release build

4_0:
	xcodebuild -target "CombineLibs (4.0)" -configuration Release build

# If you need to clean a specific target/configuration: $(COMMAND) -target $(TARGET) -configuration DebugOrRelease -sdk $(SDK) clean
clean:
	-rm -rf build/*

test-3:
	GHUNIT_CLI=1 xcodebuild -target "Tests (3.0)" -configuration Debug -sdk iphonesimulator3.2 build


test-4:
	GHUNIT_CLI=1 xcodebuild -target "Tests (4.0)" -configuration Debug -sdk iphonesimulator4.0 build
	
