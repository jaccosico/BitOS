***************************************************************************

accessing camera library

copy & paste "camera" folder to drive C:

open netbeans > right click BiTOS project > properties > run > vm options

	copy & paste -Djava.library.path="C:\camera\build\java\x64"

		make sure "camera" folder is located directly at drive C:

add opencv-249.jar to libraries of the project

	this can be found at C:\camera\build\java

add these lines of code to OS_Frame (position on comment)

	import org.opencv.core.Core; // import section
	
	System.loadLibrary(Core.NATIVE_LIBRARY_NAME); // main method

done

***************************************************************************