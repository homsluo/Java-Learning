# JavaBean

## Rules:

**1.** A JavaBean must have a public, no-argument constructor.

**2.** The JavaBean class must have getter and setter.

**3.** The JavaBean class should implement the Serializable interface.


# Accessing JavaBeans in JSP

## Basic JSP tags:

**1.** ```<jsp:useBean id="bean's name" scope="bean's scope" class="bean's class name"/>```  

**2.** ```<jsp:setProperty name="bean's id" property="property name" value="value">```  

**3.** ```<jsp:getProperty name="bean's id" property="property name"/> ```

## Tag Rules:

* JSP bean tags use **XML syntax** - must include a slash to close  
* **scope** controls how long the bean object is available
  - page - current page only - stored in pageContent object  
  
  - request - all components with access to current request object  
  
  - session - all components with access to current session object  
  
  - application - all components that have access to ServletContext object  
