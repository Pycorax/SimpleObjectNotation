# Simple Object Notation
Simple Object Notation (SON) is inspired by JavaScript Object Notation (JSON) and aims to offer the bare basic capabilities of JSON using simple curly braces and square brackets.

## Syntax
    {
    	# This is level 1
    	[Name] Body
    	[Value] Metal
    	
    	{
    		# This is level 2
    		[Name] Level2
    		{
    			# This is level 3
    			[Name] Level3
    			[Value] "Plastic SPACING"
    		}
    	}
    	
    	{
    		[Name]Level2-2
    	}
    }

## Compatibility
SONIO is written in **C++98** and is compatible with any version of **Visual Studio 2010 and up**.
	
## Usage
The code-wise implementation of SON is SON Input-Output (SONIO). SONIO is designed as a C++ static library that can be linked to your C++ Visual Studio project for use. Data stored in a SON file is stored in a tree data structure known as a `Branch`.

### Reading
`LoadSON()` allows you to generate a `Branch` object from a SON file.

### Writing
`WriteSON()` allows you to generate a SON file from a `Branch` object.

### Future Development
In future, an interface class will be provided to allow read/writing from any C++ object to a SON files without requiring the use of `Branch` objects for manual translation.