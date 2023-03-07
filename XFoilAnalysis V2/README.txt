Q: Is aileron deflection sufficient 

1.) Open a command prompt NOT powershell

2.) generate the airfoils at various deflections
	
		C:\Users\Windows> cd "C:\Users\Windows\Desktop\OmniResources\Semesters\6 Spring 2023 Omnibus\0 Construct and Exercises"

		C:\Users\Windows\Desktop\OmniResources\Semesters\6 Spring 2023 Omnibus\0 Construct and Exercises> xfoil <flapmaker.txt> out

		C:\Users\Windows\Desktop\OmniResources\Semesters\6 Spring 2023 Omnibus\0 Construct and Exercises>xfoil ag36_f05.dat

3.) exit out of the previous step with CTRL+C for each airfoil deflection case, run the generator:

		C:\Users\Windows> cd "C:\Users\Windows\Desktop\OmniResources\Semesters\6 Spring 2023 Omnibus\0 Construct and Exercises"

		C:\Users\Windows\Desktop\OmniResources\Semesters\6 Spring 2023 Omnibus\0 Construct and Exercises>xfoil < af_00deg.txt > output.txt

4.) Repeat this process for elevator and rudder

5.) Compute hinge moment
	Open the generated <output> file and CTRL+F for Hinge Moment
	Refer to AVL file for Spans or check as listed below if necessary:
		NOTE: Span = Chord Length = <Chord>
		Aileron = 0.447
		Elevator = 0.222
		Rudder = 0.295
	You need only multiply the moment per unit span by the span above for a value in Newton Meters

	HT Total Chord is 0.99457 at 15 degrees
	HT Total Chord is 0.99760 at 10 degrees
	HT Total Chord is 0.99941 at 05 degrees
	HT Total Chord is 1.00002 at 00 degrees

	AG Total Chord is 0.99219 at 15 degrees
	AG Total Chord is 0.99611 at 10 degrees
	AG Total Chord is 0.99882 at 05 degrees
	AG Total Chord is 1.00031 at 00 degrees
    