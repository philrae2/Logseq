---
title: Python Basics + [[EDX]]
---

- String Operations
	 - You can use double quotes or single quotes.

	 - Can contain spaces, numbers, letters, or special characters

	 - Can be thought of a sequenced__ index__
		 - Each element in the array can be accessed by String[#]

		 - We can use negative indexing. The last element of the index is -1

	 - __slicing__
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FGVLOgZ6Gjo.png?alt=media&token=3a1e559f-b991-4753-b633-22b13e5dac36)

	 - Stride
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FDmD3HR8Azn.png?alt=media&token=62a44980-baec-4e92-85f8-d7d241a546e6)

	 - Replace within a string with the method string.replace("old text", "new text")
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2Fm_o6HTQ8cV.png?alt=media&token=31ca26d5-7d0c-48f7-ad45-888f257e3c5e)

	 - Concatenate with "+"

	 - Strings are immutable and cannot be changed
		 - To manipulate the string it has to be manipulated and placed in another variable for example StringB = StringA.upper() - creates a new uppercase string

	 - \n = new line 

	 - \t = tab

	 - Searching within a string
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FHm-9Rfcypu.png?alt=media&token=fda6fdd2-d48b-4290-94f4-a964735970d5)
			 - A false value is -1

- Data Structures
	 - Lists
		 - Mutable

		 - L = [ data, data]

		 - Can contain strings, integers, float, other lists and other data structures

		 - Index
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FmsmCSM3q46.png?alt=media&token=d76364b2-f44a-463a-91a4-fa29e85050c6)

			 - We can also use a negative index, -3, -2, -1

			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2F2z78oOxWew.png?alt=media&token=570939f9

		 - Slicing
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2F2z78oOxWew.png?alt=media&token=570939f9-1bce-4284-80a4-bae5742bafa3)
				 - When referring to the last item, it is one larger the index.

		 - Concatenate:
			 - Using extend method
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FLe6DFzFYXV.png?alt=media&token=95bcbcbc-7595-4983-bb25-e36b16959222)

			 - Using the append method
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2Fe5HuE386PP.png?alt=media&token=2dd7544d-eb53-4833-942b-9d294d22a56c)

		 - Deleting elements
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FITBTZcn_ZP.png?alt=media&token=b95100f5-271e-44d2-8bb9-3fb5094f4a0e)

		 - Converting strings
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2F_93LQ6ZfDD.png?alt=media&token=8fd80927-6b1a-4831-b3e0-745dbc3a6b3b)

			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FS8E1pr606D.png?alt=media&token=6e51a3ea-d62a-4044-a79b-d842d5ae65c9)
				 - We can separate the list using a delimiter

		 - Aliasing
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FkbQlwOyqyr.png?alt=media&token=bf4a1c0c-78dd-4cd5-b6fe-b17bf922cbd8)

			 - When making changes in A it will also change B

		 - Cloning - Creates a clone of an original list that can be modified indepedently of the original
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FT5NCV1RB3S.png?alt=media&token=7ba00e09-6ea3-4d2c-82c5-2577143d1d9b)

		 - To sort you can used the __sorted()__ function. sorted(tuple_or_list)

	 - Tuples
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2Fc7BcZFryeq.png?alt=media&token=6c983ead-b3bb-4050-88b3-72c2c6458f46)

		 - Immutable
			 - We can't change data. To manipulate a tuple we have to create a new tuple. For example sorting a tuple would be tuple2 = sort (tuple)

		 - T = (data, data)

		 - Can contain strings, integer and float

		 - Accessed by an index

		 - You can add tuples tuple2 = tuple1 + ("disco", 1)
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FOeE9UfvTSM.png?alt=media&token=3236fdbf-4821-446b-a8b4-4b99588b5589)

		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2F14opwzpUEc.png?alt=media&token=70f348f2-94c9-4813-ad3d-1c82362aa5d9)
			 - The last index is one larger when slicing tuples

		 - Use the len command to obtain the length of a tuple

		 - You can nest a tuple within a tuple and access them as shown
			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FB1tKq9R08z.png?alt=media&token=af727a75-76ec-42b9-af66-7c4a0c84a816)
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FOuKPIjojMf.png?alt=media&token=72d9da75-f150-4fba-b6df-d3c067a7dbdc)

				 - We can access the individual letters 
					 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2Fk2_Yjb9vfr.png?alt=media&token=c467f5f2-6257-435c-987e-7e27ed9182ed)

				 - We can find the index by using the method tuple.index ("stored_data")
					 - 

	 - Sets
		 - Characteristics
			 - Can contain different data types

			 - They are unordered. They do not record element position

			 - They contain unique elements. Cannot contain duplicates

		 - Creating a set use setName = {data, data, data}
			 - We can typecast a list into a set by using set(list_name)

			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FNFnGBYZ8A7.png?alt=media&token=b7892495-8c42-4bc4-ba3d-4a629a056c4e)

		 - Adding to a set we can use the .add method. ex. setName.add("data")

		 - We can remove using the method .remove. Ex: setName.remove ("remove")

		 - Search
			 - We can search for an item in a set with the __in__ function
				 - "text" in setName

				 - If in item is in the set, then we will get a true, if not we will get a false

		 - Intersection
			 - We can find the elements that are intersecting between two or more sets using the &
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FUSYHMQi9TE.png?alt=media&token=519997ac-c888-4608-b50a-61719e6ec4e9)

		 - Subset and superset
			 - To check if a set is a subset of another set use the issubset method
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FT8JT1CJWyx.png?alt=media&token=55b9935f-897a-4aea-a768-f21cd77fb407)

			 - We can check the reverse with album_set_1.issuperset(albumt_set3)

			 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FyV65Ktpaxb.png?alt=media&token=e4277abd-cafa-4554-ab07-d834fb5ea015)

		 - Union
			 - To find the union between two sets use the method .union
				 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2F7gpzON4dWW.png?alt=media&token=90c21a25-544a-409a-90e7-67f66713b8ce)

		 - Difference
			 - We can find the difference of a subset, meaning only the unique elements from one subset to another using the difference method. ex. album_set1.difference(album_set2) 

	 - Dictionaries
		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FGEvoN21WGS.png?alt=media&token=8b1ba05b-7f71-49b7-be3e-8f2be708c568)

		 - In summary, like a list, a dictionary holds a sequence of elements. Each element is represented by a key and its corresponding value. Dictionaries are created with two curly braces containing keys and values separated by a colon. For every key, there can only be one single value, however, multiple keys can hold the same value. Keys can only be strings, numbers, or tuples, but values can be any data type.

		 - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2FReligion%2FGKjhW1gee7.png?alt=media&token=9573db97-7c3e-49f6-a433-bfba44b28e69)

		 - To create a diction use {} with colon and commas to separate corresponding values
			 - Dict = {"key1": 1, "key2": "2", "key3": [3, 3, 3], "key4": (4, 4, 4), ('key5'): 5, (0, 1): 6}

		 - **Accessing keys**: Dict["key1"]
			 - Dict[(0, 1)] = 6

		 - Retrieving the list of **keys** by using .key method. Ex. release_year_dict.keys() 

		 - **Values** - we can get all the values from the dictionary using the .values method. ex. release_year_dict.values() 

		 - **Append** - release_year_dict['Graduation'] = '2007'

		 - **Delete** - we can delete values by key. ex: del(release_year_dict['Thriller'])

		 - We can check if a key is in the dictionary by using   __in__. Ex: 'The Bodyguard' in release_year_dict
