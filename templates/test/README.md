# test Template
Template for creating an empty junit 4 test.  This template will also import hamcrest core matchers as well as junit asserts to make them readily available for testing.  This is done with the * import approach because the intended use case is to have organize imports on during save actions.  If this is not the desired behavior, just remove the imports from the template.

#### Keyword
```
test
```

#### Replacement Value
```
@${testType:newType(org.junit.Test)}
public void test${methodUnderTest}_${scenario}()  
{
	${cursor}
}
${staticImport:importStatic('org.hamcrest.CoreMatchers.*', 'org.junit.Assert.*')}
```

