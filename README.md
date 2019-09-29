### orienter
---
https://github.com/OrienteerBAP/Orienteer

```java
// orienteer-core/src/test/java/org/orienteer/core/method/TestFilter.java
package org.orienteer.core.method;

public class TestFilter implements IMethodFilter{
  
  private String filterData;
  
  @Override
  public IMethodFilter setFilterData(String filterData) {
    this.filter = filterData;
    return this;
  }
  
  @Override
  public boolean isSupportedMethod(IMethodContext dataObject) {
    return (dataObject.getCurrentWidget()==null &&
      dataObject.getDisplayObjectModel()==null &&
      "testData".equals(filterData)
      );
  }
}

```

```
```

```
```
