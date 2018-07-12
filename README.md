[PARAMETER feature](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature) & [PARAMETER StepDefinition](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java)

-----	

[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L3): Delimiter annotation scenario

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L20): the user names are jane,john,colin,alice --> Convert to List<String>.

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L26): the users are jane,john,colin,alice	--> Convert to List< dataobject.User>. User has a single argument constructor.
	
-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L8): Format annotation scenario	

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L32): the date is 2017-11-05T09:54:13	--> Convert to java.util.Date.
	
-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L10): Transformer annotation scenario

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L38): the name is 'John Mich Arthur Doe' --> Convert to custom dataobject.FullName. FullName does NOT have a single argument constructor.

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L44): the amount is $91.63 --> Convert to custom dataobject.Money. Money does NOT have a single argument constructor.
	
-----	

[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L14): Single argument constructor scenario	

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L50): the user name is John Doe --> Convert to custom dataobject.User. 

-----	

[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L17): NO single argument constructor scenario

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L56): the professor is John Doe --> Convert to custom dataobject.Professor. Professor does NOT have a single argument constructor.

-----	

[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/parameter.feature#L20): Enum scenario

[Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/ParameterStepDefinition.java#L62): the professor level is ASSOCIATE --> Convert to custom dataobject.ProfLevels enum.

-------------------------------------------------------------------

[DATATABLE feature](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature) & [DATATABLE StepDefinition](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java)

-----	

[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L3): List of primitive --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L23) Convert to List<List<String>>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L8): List of object containing primitive fields --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L29) Convert to List<LecturePrimitive>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L14): List of object containing primitive & enum fields --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L35) Convert to List<LecturePrimitiveEnum>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L20): List of object containing object fields --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L41) Convert to List<Lecture>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L26): Transpose List of object containing object fields --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L47) Convert to List<Lecture> with Transpose annotation.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L34): List of object containing object fields with no table header --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L53) Convert to List<LectureLite>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L39): Map of primitive key and value --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L62) Convert to Map<String,String>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L44): Map of object key and enum value --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L68) Convert to Map<Professor,ProfLevels>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L49): Map of primitive key and object value --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L74) Convert to Map<String, Lecture>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L54): Map of object key and value --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L83) Convert to Map<Lectureid, Lecture>.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L59): Transpose Map of object key and value --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L89) Convert to Map<Lectureid, Lecture> with Transpose annotation.

-----	
	
[Scenario](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/resources/features/datatable.feature#L68): Whole table to single object Lectures --> [Step](https://github.com/grasshopper7/cuke2-parameter-datatable/blob/master/cuke2-parameter-datatable/src/test/java/stepdef/DataTableStepDefinition.java#L95)Convert to object Lectures.
